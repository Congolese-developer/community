# Contributing to Congolese Developers

First of all — **thank you!** 🇨🇩 Every contribution, big or small, helps build the
Congolese technology community.

This guide is written for **beginners**. If you have never contributed to an open-source
project before, you are in the right place: follow the steps one by one.

> 🇫🇷 Vous préférez le français ? Un résumé est disponible dans
> [docs/fr/README.md](docs/fr/README.md#-contribuer). Vous pouvez aussi ouvrir vos issues et
> discussions en français.

---

## Table of Contents

- [Ways to contribute](#ways-to-contribute)
- [Before you start](#before-you-start)
- [Step-by-step: your first Pull Request](#step-by-step-your-first-pull-request)
  - [1. Fork the repository](#1-fork-the-repository)
  - [2. Clone your fork](#2-clone-your-fork)
  - [3. Create a branch](#3-create-a-branch)
  - [4. Make your changes](#4-make-your-changes)
  - [5. Commit your changes](#5-commit-your-changes)
  - [6. Push and open a Pull Request](#6-push-and-open-a-pull-request)
  - [7. Respond to the review](#7-respond-to-the-review)
- [Commit message convention](#commit-message-convention)
- [Branch naming](#branch-naming)
- [How to report a bug](#how-to-report-a-bug)
- [How to suggest a feature or improvement](#how-to-suggest-a-feature-or-improvement)
- [How to propose a new project](#how-to-propose-a-new-project)
- [Writing style for documentation](#writing-style-for-documentation)
- [Getting help](#getting-help)

---

## Ways to contribute

You don't need to write code to contribute. All of these are valuable:

| Contribution | Examples |
|:--|:--|
| 📝 **Documentation** | Fix a typo, clarify a sentence, add a guide or resource |
| 🌍 **Translation** | Translate documents into French (or another language spoken in the DRC) |
| 🐛 **Bug reports** | Report a broken link, a wrong instruction, a template that doesn't work |
| 💡 **Ideas** | Suggest improvements to the community or its tools |
| 🧩 **Projects** | Propose or join an open-source project |
| 💬 **Support** | Answer questions from other members in Discussions |
| 🎨 **Design** | Improve the logo, banners or visual identity |

---

## Before you start

1. **Read the [Code of Conduct](CODE_OF_CONDUCT.md).** By participating, you agree to follow it.
2. **Search first.** Check existing [issues](../../issues) and [discussions](../../discussions)
   to avoid duplicates.
3. **For big changes, talk first.** Open an issue or a discussion before investing a lot of
   time, so maintainers can confirm the change is wanted.
4. **Install Git.** If Git is new to you, follow the
   [Getting Started guide](docs/getting-started.md) first.

---

## Step-by-step: your first Pull Request

A **Pull Request** (PR) is how you propose a change. You copy the project (fork), change your
copy, then ask maintainers to "pull" your change into the original.

### 1. Fork the repository

Click the **Fork** button at the top-right of this repository's page on GitHub. This creates
your own copy at `https://github.com/<your-username>/community`.

### 2. Clone your fork

Download your copy to your computer:

```bash
git clone https://github.com/<your-username>/community.git
cd community
```

Then connect it to the original repository (called **upstream**) so you can receive
future updates. Copy the original repository's URL from the green **Code** button on its
GitHub page:

```bash
git remote add upstream <original-repository-url>
git remote -v   # check: you should see "origin" (your fork) and "upstream" (original)
```

### 3. Create a branch

Never work directly on `main`. Create a branch for each change:

```bash
git checkout main
git pull upstream main          # get the latest version
git checkout -b docs/fix-faq-typo
```

See [Branch naming](#branch-naming) for how to name your branch.

### 4. Make your changes

Edit the files with any text editor (VS Code is a good free choice). Keep each PR focused on
**one** topic — small PRs are reviewed faster.

Check your work before committing:

- Preview Markdown files (in VS Code: `Ctrl+Shift+V`).
- Make sure links work.
- Re-read your text for spelling.

### 5. Commit your changes

```bash
git status                      # see which files changed
git add docs/faq.md             # add specific files (or "git add ." for all)
git commit -m "docs: fix typo in FAQ"
```

Follow the [commit message convention](#commit-message-convention).

### 6. Push and open a Pull Request

```bash
git push origin docs/fix-faq-typo
```

Go to your fork on GitHub. A yellow banner will offer **Compare & pull request** — click it,
fill in the [pull request template](.github/PULL_REQUEST_TEMPLATE.md), and submit.

### 7. Respond to the review

A maintainer will review your PR. They may ask for changes — this is normal and part of
learning! Make the changes on the same branch, then:

```bash
git add .
git commit -m "docs: apply review suggestions"
git push origin docs/fix-faq-typo
```

The PR updates automatically. Once approved, a maintainer will merge it. 🎉

> **Keeping your fork up to date:**
> ```bash
> git checkout main
> git pull upstream main
> git push origin main
> ```

---

## Commit message convention

We use [Conventional Commits](https://www.conventionalcommits.org/). Each commit message
starts with a **type**, a colon and a short description in the imperative mood
("add", not "added").

```text
<type>: <short description>
```

| Type | Use it for | Example |
|:--|:--|:--|
| `feat` | A new feature | `feat: add join community issue template` |
| `fix` | A bug fix | `fix: correct broken link in README` |
| `docs` | Documentation only | `docs: add Flutter resources to getting started` |
| `refactor` | Restructuring without changing behavior | `refactor: reorganize docs folder` |
| `test` | Adding or updating tests | `test: add link checker test` |
| `chore` | Maintenance tasks | `chore: update issue labels` |

Tips:

- Keep the first line under **72 characters**.
- Use English for commit messages so everyone can read the history.
- Add a longer explanation after a blank line if needed.

---

## Branch naming

Use the commit type as a prefix, then a short description with hyphens:

```text
feat/project-directory-table
fix/broken-faq-link
docs/french-getting-started
chore/update-labels
```

---

## How to report a bug

Found something broken — a dead link, a wrong instruction, a template that fails?

1. Search [existing issues](../../issues) to see if it is already reported.
2. Open a new issue with the **🐛 Bug Report** template from [New issue](../../issues/new/choose).
3. Describe the bug, the steps to reproduce it, what you expected and what actually happened.

Bugs in a specific community project should be reported in **that project's repository**.

> 🔐 Do **not** report security vulnerabilities or Code of Conduct violations in public
> issues. See [Enforcement](CODE_OF_CONDUCT.md#enforcement) for private reporting.

---

## How to suggest a feature or improvement

- **New feature** for the community hub (a new template, a new guide, a new tool) →
  use the **✨ Feature Request** template.
- **Improvement** to something that already exists (clearer docs, better process) →
  use the **🔧 Improvement Suggestion** template.
- **Not sure yet?** Start a conversation in the *Ideas & Proposals* category of
  [Discussions](../../discussions).

---

## How to propose a new project

Have an idea for an open-source project that could serve the DRC or the world?

1. Check the [project directory](docs/projects.md) to see if something similar exists.
2. Optionally, discuss the idea in *Ideas & Proposals* in [Discussions](../../discussions).
3. Open an issue with the **🚀 Project Proposal** template.
4. The community gives feedback; administrators decide whether to create a repository in the
   organization.

The full lifecycle is described in [docs/projects.md](docs/projects.md#how-a-project-is-created).

---

## Writing style for documentation

- Write in **simple, clear English**. Many readers use English as a second or third language.
- Prefer short sentences and lists.
- Explain technical terms the first time you use them.
- Use [GitHub Markdown](https://docs.github.com/en/get-started/writing-on-github): headings,
  lists, code blocks with a language (` ```bash `).
- Use relative links between files (`docs/faq.md`, not full URLs).
- Never add contact details, social links or projects that don't really exist.

---

## Getting help

Stuck at any step? That's completely fine.

- Ask in the *Help & Support* category of [Discussions](../../discussions).
- Comment on your Pull Request — maintainers are happy to guide you.
- Read the [FAQ](docs/faq.md).

**Welcome to the community — we're glad you're here.** 🇨🇩
