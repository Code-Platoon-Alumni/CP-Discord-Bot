# CONTRIBUTING

Thanks for helping build the Code Platoon Alumni Discord Bot!

> **⚠️ Important:** This project is limited to **Code Platoon Alumni only**. You must be a graduate of Code Platoon to contribute to this repository.

---

## 📜 Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md).  
By participating in this project, you agree to abide by its terms.

---

## How to contribute
1. **Request assignment** before starting work:
   - Comment on the issue you want to work on with "I'd like to work on this"
   - Wait for a maintainer to assign you to the issue
   - Issues will be assigned on a first-come, first-served basis
2. **Fork** the repo and create a feature branch after being assigned.
3. Keep PRs **small and focused**. Include rationale and screenshots for docs/UI-related changes.
4. Write clear commit messages (e.g., `docs: add README section for stateless audits`).

## Ground rules
- **Request assignment first** - Don't start work without being assigned to an issue
- Follow the **Code of Conduct**.
- Avoid committing secrets.
- Prefer issues before large changes for alignment.
- Reference related issues in your PR description.
- If you're assigned to an issue but can't complete it, please comment to let maintainers know so it can be reassigned.

## Development (no-code phase)
- This repo is in **planning mode**. Use issues to propose the initial Python scaffold (`discord.py`, `apscheduler`) and stateless audit flow.

---

## 📋 Issue Assignment Process

### For Contributors:
1. **Verify eligibility** - Ensure you are a Code Platoon Alumni
2. **Browse available issues** - Look for issues labeled `good first issue` or `help wanted`
3. **Request assignment** - Comment "I'd like to work on this" on the issue
4. **Wait for assignment** - A maintainer will assign you and may provide additional context
5. **Work on your assigned issue** - Create your fork and feature branch after assignment
6. **Submit your PR** - Reference the issue number in your PR description using #issueNumber

### For Maintainers:
- **Verify contributor eligibility** - Confirm contributors are Code Platoon Alumni before assignment
- Assign issues promptly to requesting contributors
- Provide clear acceptance criteria and context when assigning
- Use issue labels to indicate status: `assigned`
- Reassign stale issues after 7 days of inactivity (with notice to the assignee)

---

## 🧱 Suggested Tech Stack (Python)
- **Language:** Python 3.11+
- **Discord SDK:** `discord.py` (2.x)
- **Scheduler:** `apscheduler` (for cron-like jobs)
- **Persistence:** None (stateless audits based on join date)
- **Hosting:** Railway / Render / Docker on VPS
- **Config:** `.env` + `python-dotenv`
- **Logging:** `logging`
- **Testing:** `pytest`
- **CI:** GitHub Actions (lint, test)

---

## 🧭 Repo Layout (planned)
```
/ (root)
  ├─ .github/
  │   ├─ ISSUE_TEMPLATE/
  │   │   ├─ bug_report.yml
  │   │   ├─ feature_request.yml
  │   │   └─ task.yml
  │   └─ workflows/
  │       └─ ci.yml
  ├─ bot/ (to be added)
  ├─ .env.example
  ├─ CONTRIBUTING.md
  ├─ CODE_OF_CONDUCT.md
  ├─ SECURITY.md
  ├─ PRIVACY.md
  ├─ LICENSE
  └─ README.md
```

---

## 🚀 Getting Started (stub)
1. **Prereqs:** Python 3.11+, pip, virtualenv.
2. **Create bot** in Discord Developer Portal → enable SERVER MEMBERS intent.
3. Create `.env` from [`.env.example`](.env.example):
4. Install deps: `pip install -r requirements.txt`

---

## 📂 Issue Templates
*(bug_report.yml, feature_request.yml, task.yml — same as current version)*

---

## 🗓️ Roadmap
- [ ] Python project init + `discord.py` client
- [ ] Slash command registration
- [ ] Event announcement listeners
- [ ] Monthly rundown job
- [ ] Stateless name policy audit job
- [ ] DM templates and kicking workflow
- [ ] CI pipeline setup
- [ ] Dockerfile and deploy docs

---

## 🔐 Security & Privacy
- Never commit secrets; use environment variables.
- Scope the bot token to least privileges.
- Avoid storing DM contents.
- Provide a `/privacy` command and a `PRIVACY.md`.


