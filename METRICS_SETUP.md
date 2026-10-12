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
- **Authored commits:** commits attributed by GitHub to the account on each owned repository's default branch. This is not a count of every commit by every contributor, and it can differ from the profile contribution graph.
- **Last 30 days:** authored commits dated within the last 30 days.
- **Active repositories:** owned repositories with at least one attributed commit in the last 30 days.
- **Recent public work:** latest commit subjects from public repositories only.
- **Private work:** included in aggregate counts, but private repository names and commit messages are not published.

GitHub's commit API applies GitHub's author attribution and repository history rules. Commits in other branches, unlinked author emails, and inaccessible repositories may not be included. Treat these metrics as transparent repository-history counts, not a universal count of every Git operation ever made on every machine.
