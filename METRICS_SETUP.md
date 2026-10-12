# Profile metrics setup

This repository's public profile README can show live, verified repository and commit metrics without exposing private project names or commit messages.

## Required repository secret

Open **Settings → Secrets and variables → Actions → New repository secret** in `janarthananRaja/janarthananRaja`.

### `PROFILE_READ_TOKEN`

Create a fine-grained personal access token with your account as the resource owner and access to **all repositories you own** (including private repositories).

Permissions:
- **Metadata:** Read-only
- **Contents:** Read-only

This token is used only to count authored commits and inspect dates. It is never printed or written to the generated README.

### Why there is no write token secret

The workflow uses GitHub Actions' short-lived `GITHUB_TOKEN` to update this profile repository. Its permissions are limited in the workflow to `contents: write` for this repository only. This avoids storing a second long-lived personal access token.

## Run it

1. Add `PROFILE_READ_TOKEN` as a repository secret.
2. Open **Actions → Refresh engineering profile metrics**.
3. Select **Run workflow**.
4. Check the run logs for the summary. The README metrics update when the workflow succeeds.

The workflow also runs daily.

## What the numbers mean

- **Repositories:** non-archived repositories owned by the account, public and private. This is a repository count, not a guarantee that each repository represents one distinct project.
- **All-time authored commits:** unique commits attributed by GitHub to the configured author identities across every branch of each owned, non-archived repository with history. Commits are deduplicated by repository + commit SHA, so shared commits across branches count once.
- **Last 30 days:** commits whose author timestamp falls within the rolling 30-day window ending at the workflow snapshot time. All-time and recent metrics use the same repositories, identities, and deduplication rules.
- **Older than 30 days:** all-time authored commits minus recent authored commits. These two periods partition the same all-time set.
- **Active repositories:** distinct owned repositories with at least one qualifying authored commit in the last 30 days.
- **Configured author identities:** `janarthananRaja` and `Janarthanan9751`. Add another identity only after verifying it belongs to the profile owner.
- **Recent public work:** latest commit subjects from public repositories only.
- **Private work:** included in aggregate counts, but private repository names and commit messages are not published.

The workflow scans every branch exposed by the read token and fails closed if branch/history access fails, rather than publishing partial totals. GitHub's commit API still applies author attribution rules: commits using an unlinked email or an unconfigured username may not be included. The rolling window includes its lower boundary and excludes commits dated after the snapshot time. These are repository-history counts, not a count of every Git operation ever made on every machine.
