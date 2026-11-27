# Governance

This document describes how **Congolese Developers** is organized, who is responsible for
what, and how decisions are made. Our goal is simple: **transparent decisions and clearly
documented responsibilities**, so that anyone can understand how the community works and how
to take on more responsibility.

> 🇫🇷 Un résumé en français est disponible dans
> [docs/fr/README.md](docs/fr/README.md#️-gouvernance).

---

## Table of Contents

- [Principles](#principles)
- [Roles](#roles)
  - [Founder](#founder)
  - [Organization Administrators](#organization-administrators)
  - [Project Maintainers](#project-maintainers)
  - [Contributors](#contributors)
  - [Community Members](#community-members)
- [Summary of permissions](#summary-of-permissions)
- [Decision-making](#decision-making)
- [Becoming a maintainer or administrator](#becoming-a-maintainer-or-administrator)
- [Stepping down and inactivity](#stepping-down-and-inactivity)
- [Conflict resolution](#conflict-resolution)
- [Changing this document](#changing-this-document)
- [Current role holders](#current-role-holders)

---

## Principles

1. **Openness** — Discussions and decisions happen in public (issues, pull requests,
   discussions), except for private matters such as Code of Conduct reports.
2. **Merit and contribution** — Responsibility is earned through sustained, constructive
   participation, not through status, title or location.
3. **Inclusivity** — Every province, technology and experience level has a voice.
4. **Documentation** — Important decisions are written down and linked so they can be found
   later.
5. **Service** — Leadership roles exist to serve the community, not to control it.

---

## Roles

### Founder

The person who created the community.

- Establishes and communicates the community **vision**.
- **Coordinates** the organization and its overall direction.
- **Appoints the initial maintainers** and administrators.
- Acts as final tie-breaker when consensus cannot be reached (see
  [Decision-making](#decision-making)).

### Organization Administrators

Trusted members who keep the GitHub organization running.

- Manage **GitHub organization settings** (Discussions, labels, teams, security settings).
- Manage **permissions** — add members, create teams, grant repository access.
- **Supervise repositories** — create new project repositories, archive inactive ones.
- Enforce the [Code of Conduct](CODE_OF_CONDUCT.md).
- Welcome new members who open a *Join the Community* issue.

### Project Maintainers

Leaders of individual community projects.

- **Manage** one or more project repositories and their roadmap.
- **Review and merge Pull Requests**.
- **Triage issues** — label, prioritize, close duplicates.
- Keep the project's entry in the [project directory](docs/projects.md) up to date.
- Mentor contributors and identify future maintainers.

### Contributors

Anyone who has contributed to a community repository.

- **Submit code** through Pull Requests.
- **Improve documentation** and translations.
- **Report bugs** and suggest improvements.
- **Participate in discussions** and reviews.

### Community Members

Everyone who has joined the community.

- **Share ideas** and experience.
- **Participate** in discussions.
- **Help newcomers** find their way.

---

## Summary of permissions

| Role | GitHub permission (typical) | Can merge PRs | Can manage org settings |
|:--|:--|:--:|:--:|
| Founder | Organization owner | ✅ | ✅ |
| Organization Administrator | Organization owner | ✅ | ✅ |
| Project Maintainer | `Maintain` or `Admin` on their project | ✅ (own project) | ❌ |
| Contributor | `Read` (contributes through forks) or `Triage` | ❌ | ❌ |
| Community Member | Organization member (optional) | ❌ | ❌ |

> Organization owners should always be **at least two** trusted people, so the community
> never depends on a single account.

---

## Decision-making

We use **lazy consensus**: a proposal is accepted if no one raises a reasoned objection
within the review period.

| Type of decision | Where | Who decides | Minimum review period |
|:--|:--|:--|:--|
| Small changes (typos, docs fixes) | Pull Request | One maintainer approval | None |
| Changes inside a project | Project's issues / PRs | That project's maintainers | Defined by the project |
| New community project | *Project Proposal* issue | Organization Administrators | 7 days of community feedback |
| Changes to community-wide documents (README, guidelines) | Pull Request | Two approvals, one from an administrator | 3 days |
| Changes to Code of Conduct or Governance | Pull Request + announcement in Discussions | Administrators by consensus | 14 days |
| New administrators or maintainers | Issue or private discussion among admins | Administrators, confirmed by the Founder | 7 days |

When consensus cannot be reached:

1. The discussion moves to a dedicated GitHub Discussion so all arguments are visible.
2. Administrators hold a simple majority vote and record the result.
3. If the vote is tied, the Founder makes the final decision and explains it publicly.

All significant decisions are **linked from the related issue or discussion** so they remain
traceable.

---

## Becoming a maintainer or administrator

There is no application form — responsibility grows naturally:

1. **Contribute regularly** — Pull Requests, reviews, answers in Discussions.
2. **Show good judgment** — respectful communication, helpful reviews, respect for the
   Code of Conduct.
3. **Get nominated** — any maintainer or administrator can nominate you, or you can express
   interest yourself.
4. **Approval** — administrators decide following the process in
   [Decision-making](#decision-making), and the nomination is announced publicly.

---

## Stepping down and inactivity

- Anyone can step down from a role at any time by informing the administrators. Thank you
  for your service!
- Maintainers or administrators inactive for **6 months** may be contacted; without a reply
  after **30 days**, their elevated permissions may be removed. They can regain them later.
- Former role holders are listed as **Emeritus** to recognize their contributions.

---

## Conflict resolution

1. Try to resolve disagreements directly and respectfully in the issue or PR.
2. If that fails, ask a neutral maintainer or administrator to mediate.
3. Conduct-related conflicts follow the [Code of Conduct enforcement process](CODE_OF_CONDUCT.md#enforcement).

---

## Changing this document

Changes to this document follow the "Code of Conduct or Governance" row in
[Decision-making](#decision-making): a Pull Request, an announcement in Discussions, and a
14-day review period.

---

## Current role holders

> 📌 This table must be filled in by the Founder when the organization is published.
> Only list real people who have accepted the role.

| Role | GitHub username | Since |
|:--|:--|:--|
| Founder | *To be completed* | — |
| Organization Administrators | *To be completed* | — |
| Project Maintainers | See each project in the [project directory](docs/projects.md) | — |
