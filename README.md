<!--
  JANARTHANAN RAJA | ENGINEERING PORTFOLIO
  Visual-first. Evidence-led. Private work remains private.
-->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=210&color=0:07111F,48:102A40,100:00D9FF&text=JANARTHANAN%20RAJA&fontColor=F2FAFF&fontSize=42&fontAlignY=37&desc=SOFTWARE%20ENGINEER%20%20%E2%80%A2%20%20FULL-STACK%20BUILDER&descSize=14&descAlignY=59&animation=fadeIn" width="100%" alt="Janarthanan Raja — software engineer"/>

<a href="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&size=16&duration=2600&pause=800&color=55E6FF&center=true&vCenter=true&width=850&lines=Interfaces+with+intent.;APIs+with+clear+contracts.;Architecture+that+can+be+explained.;Metrics+that+can+be+verified."><img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&size=16&duration=2600&pause=800&color=55E6FF&center=true&vCenter=true&width=850&lines=Interfaces+with+intent.;APIs+with+clear+contracts.;Architecture+that+can+be+explained.;Metrics+that+can+be+verified." alt="Animated engineering principles"/></a>

<br/>

<a href="https://janarthananraja.github.io"><img src="https://img.shields.io/badge/PORTFOLIO-0B1727?style=for-the-badge&logo=firefoxbrowser&logoColor=55E6FF" alt="Portfolio"/></a>
<a href="https://github.com/janarthananRaja?tab=repositories"><img src="https://img.shields.io/badge/PROJECTS-0B1727?style=for-the-badge&logo=github&logoColor=55E6FF" alt="Projects"/></a>
<a href="https://github.com/janarthananRaja?tab=overview"><img src="https://img.shields.io/badge/ACTIVITY-0B1727?style=for-the-badge&logo=githubactions&logoColor=55E6FF" alt="Activity"/></a>

</div>

---

## The short version

<table width="100%">
<tr>
<td width="33%" align="center" valign="top">

<img src="https://img.shields.io/badge/01-UX%20%26%20UI-102A40?style=flat-square&labelColor=00BFD9" alt="UI"/>

### Build the experience

Responsive interfaces, reusable components, clear interaction states, and dashboards that help people act instead of just stare at charts.

</td>
<td width="34%" align="center" valign="top">

<img src="https://img.shields.io/badge/02-FULL--STACK-102A40?style=flat-square&labelColor=00BFD9" alt="Full stack"/>

### Connect the system

Frontend workflows tied to API contracts, business rules, authorization, relational data, and useful failure handling.

</td>
<td width="33%" align="center" valign="top">

<img src="https://img.shields.io/badge/03-ENGINEERING-102A40?style=flat-square&labelColor=00BFD9" alt="Engineering"/>

### Make it verifiable

Git-derived analytics, repository health signals, automation, security boundaries, and metrics that can be traced to evidence.

</td>
</tr>
</table>

## My engineering map

<img src="https://raw.githubusercontent.com/janarthananRaja/janarthananRaja/main/architecture-map.svg" width="100%" alt="Visual map showing frontend, API services, identity and access, data telemetry, security, reliability and verification"/>

<sub>My default mental model: user experience → API contracts → access boundaries → data → observable outcomes. Security and reliability run through every layer, not as an afterthought.</sub>

## Projects, by the problems they solve

<sub>These are representative systems I have planned, designed, implemented, or iterated on. Private projects are intentionally described by their engineering scope rather than confidential names or source details.</sub>

<table width="100%">
<tr>
<td width="50%" valign="top">

<img src="https://img.shields.io/badge/01-ENGINEERING%20INTELLIGENCE-0D1D2D?style=flat-square&labelColor=00BFD9" alt="Engineering intelligence"/>

### Engineering intelligence platform

**The problem:** raw repository activity is noisy; teams need evidence they can inspect and act on.

**What I worked on**
- Repository health and ownership signals
- Team balance, contribution matrix, and risk views
- Code hotspots and critical-file ownership concepts
- GitHub API ingestion and rate-limit handling
- Drill-down paths instead of unexplained scores

**System shape**

`GitHub API → ingestion → analysis services → verified metrics → Angular dashboard`

<sub>Angular · TypeScript · Spring Boot · GitHub API · SQL</sub>

</td>
<td width="50%" valign="top">

<img src="https://img.shields.io/badge/02-IDENTITY%20%26%20ACCESS-0D1D2D?style=flat-square&labelColor=00BFD9" alt="Identity and access"/>

### Role-aware operations platform

**The problem:** different organisational levels need different data and permissions, without relying on frontend-only restrictions.

**Architecture work**
- JWT authentication flow
- Role and granular permission mapping
- Hierarchical organisational scoping
- API-level authorization boundaries
- Explicit verification and phase-based implementation checkpoints

**System shape**

`Identity → JWT principal → roles + permissions → scoped API access`

<sub>Spring Security · JWT · RBAC · REST APIs</sub>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="https://img.shields.io/badge/03-COMMERCE%20WORKFLOWS-0D1D2D?style=flat-square&labelColor=00BFD9" alt="Commerce workflows"/>

### Multi-sided commerce

**The problem:** customers, merchants, and administrators have related data but different jobs and workflows.

**Product and system scope**
- Separate customer, merchant, and admin experiences
- Role-specific workflow design
- API-backed operations and validation
- Relational modelling for transactional data
- Clear status transitions across the product

**System shape**

`Customer app · Merchant app · Admin web → Spring Boot → PostgreSQL`

<sub>Mobile-first UX · Spring Boot · PostgreSQL</sub>

</td>
<td width="50%" valign="top">

<img src="https://img.shields.io/badge/04-OPERATIONS%20ANALYTICS-0D1D2D?style=flat-square&labelColor=00BFD9" alt="Operations analytics"/>

### KYC & analytics workspace

**The problem:** operational teams need a clear picture of verification states, queues, and exceptions.

**Interface and data work**
- Status-driven dashboards and filters
- Data grids and export flows
- KPI summaries and analytics components
- Consistent state handling across UI and API
- CSV, Excel, and PDF reporting workflows

**System shape**

`Operational records → status logic → grid + dashboard → export/report`

<sub>Angular · Angular Material · AG Grid · SQL</sub>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="https://img.shields.io/badge/05-LOCAL--FIRST%20AI-0D1D2D?style=flat-square&labelColor=00BFD9" alt="Local-first AI"/>

### Personal companion

A privacy-first Android and desktop companion exploring modular modes and user-controlled behavior.

- Offline, online, and hybrid operating modes
- Focus, driving, meeting, gaming, sleep, and low-power modes
- Kotlin Multiplatform module boundaries
- Android interface built with Jetpack Compose
- Privacy and predictable behavior as design constraints

<sub>Kotlin · Kotlin Multiplatform · Jetpack Compose</sub>

[View public repository ↗](https://github.com/janarthananRaja/personal-companion)

</td>
<td width="50%" valign="top">

<img src="https://img.shields.io/badge/06-PLATFORM%20ENGINEERING-0D1D2D?style=flat-square&labelColor=00BFD9" alt="Platform engineering"/>

### Developer tooling & integrations

Small systems and engineering utilities built around practical debugging and delivery needs.

- Email templates separated from mail-sending logic
- GitHub repository scanning and automation
- CI/build/deployment troubleshooting
- API integration and error investigation
- Native camera and media-capture experiments
- Reproducible scripts for routine maintenance

<sub>Java · Spring Boot · Thymeleaf · GitHub Actions · Docker</sub>

</td>
</tr>
</table>

## Technical capability map

<img src="https://raw.githubusercontent.com/janarthananRaja/janarthananRaja/main/engineering-stack.svg" width="100%" alt="Visual technical capability map across frontend, backend, data, architecture, and delivery"/>

<details>
<summary><strong>Open the detailed stack</strong></summary>

| Area | Tools and concepts |
|---|---|
| Frontend | Angular, TypeScript, JavaScript, HTML5, CSS3, Bootstrap, Angular Material, AG Grid, React fundamentals |
| Backend | Java, Spring Boot, REST API design, service-layer structure, validation, integration patterns |
| Data | PostgreSQL, MySQL, SQL, relational modelling, reporting, data-grid workflows |
| Identity & security | JWT flows, roles and permissions, RBAC concepts, organisational scoping, secret handling, least privilege |
| Architecture | Module boundaries, UI/API contracts, layered services, data flow, background processing concepts, graceful failure |
| Delivery & debugging | Git, GitHub Actions, Docker, CI/CD fundamentals, logs, API debugging, deployment troubleshooting |
| Mobile & desktop | Kotlin Multiplatform, Kotlin, Jetpack Compose, native Android integrations |

</details>

## How I execute

<div align="center">
<table width="100%">
<tr>
<td width="25%" align="center" valign="top">

<img src="https://img.shields.io/badge/01-DEFINE-102A40?style=flat-square&labelColor=00BFD9" alt="Define"/>

**Problem → scope**

Clarify users, permissions, workflows, edge cases, and acceptance criteria.

</td>
<td width="25%" align="center" valign="top">

<img src="https://img.shields.io/badge/02-DESIGN-102A40?style=flat-square&labelColor=00BFD9" alt="Design"/>

**Scope → architecture**

Map modules, data flow, API contracts, security boundaries, and failure paths.

</td>
<td width="25%" align="center" valign="top">

<img src="https://img.shields.io/badge/03-IMPLEMENT-102A40?style=flat-square&labelColor=00BFD9" alt="Implement"/>

**Architecture → product**

Build vertical slices, wire real data, and keep UI states aligned with backend behavior.

</td>
<td width="25%" align="center" valign="top">

<img src="https://img.shields.io/badge/04-VERIFY-102A40?style=flat-square&labelColor=00BFD9" alt="Verify"/>

**Product → evidence**

Test, inspect, document, audit mismatches, and close phases only when verified.

</td>
</tr>
</table>
</div>

### Engineering principles

<details>
<summary><strong>Metrics must be explainable</strong></summary>

No invented activity, arbitrary productivity scores, or mystery percentages. Metrics should have a defined source, calculation, scope, and drill-down path.
</details>

<details>
<summary><strong>Security belongs in the architecture</strong></summary>

Prefer least privilege, short-lived credentials, server-side authorization, explicit scoping, and no secrets in source control.
</details>

<details>
<summary><strong>Interfaces include every state</strong></summary>

Loading, empty, validation, failure, permissions, and responsive behavior are part of the feature, not cleanup for later.
</details>

<details>
<summary><strong>Execution should be observable</strong></summary>

Use clear phase checkpoints, build feedback, repeatable automation, and evidence that a feature works beyond the happy path.
</details>

## Live engineering telemetry

<!-- PROFILE_METRICS_START -->
<div align="center">

<img src="https://raw.githubusercontent.com/janarthananRaja/janarthananRaja/main/metrics.svg" width="100%" alt="Live repository and commit telemetry"/>

<sub>Automated GitHub history · Public activity is attributable · Private details are sanitized</sub>

</div>

### Recent public work

Public commit highlights will populate after the read-only repository secret is configured.

### Private engineering activity

Private work is summarized only as aggregate counts and broad work areas. Private repository names, raw commit messages, and confidential implementation details stay private.
<!-- PROFILE_METRICS_END -->

## Contribution trail

<div align="center">

<img src="https://raw.githubusercontent.com/janarthananRaja/janarthananRaja/output/contribution-snake-dark.svg" width="100%" alt="Animated GitHub contribution history"/>

<a href="https://github.com/janarthananRaja?tab=overview">Explore the native contribution graph ↗</a>

</div>

---

<div align="center">

**Make it clear. Make it useful. Prove that it works.**

<a href="https://janarthananraja.github.io">Portfolio</a> · <a href="https://github.com/janarthananRaja?tab=repositories">Public repositories</a> · <a href="https://github.com/janarthananRaja?tab=overview">GitHub activity</a>

<sub>Dark navy × electric cyan · Built around real engineering work · Private work stays private</sub>

</div>
