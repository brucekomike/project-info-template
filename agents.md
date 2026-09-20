# Project Information Template (for local codebase analysis)

Use this template to generate a project status document from a local software repository.

## 0) Output Settings

- **Default output language**: `zh_CN`
- **Rendering options**:
  - HTML
  - PDF (A4 paper)
- **Suggested output files**:
  - `project-info.html`
  - `project-info.pdf`
- **Optional rendering commands**:

```bash
pandoc agents.md -o project-info.html -V lang=zh_CN
pandoc agents.md -o project-info.pdf -V lang=zh_CN -V papersize=a4
```

## 1) Project Info

- **Project name**:
- **Repository path**:
- **Purpose / business goal**:
- **Primary users / stakeholders**:
- **Current status** (planned / active / maintenance):
- **Main tech stack** (languages, frameworks, databases):
- **Key modules / services**:
- **Critical dependencies**:
- **Owner / team**:
- **Last updated**:

## 2) Git Repository Status

- **Current branch**:
- **Tracking remote branch**:
- **Default branch**:
- **Working tree status** (clean / dirty):
- **Uncommitted changes summary**:
- **Latest commit** (hash, author, date, message):
- **Ahead / behind remote**:
- **Open release tags / versions**:
- **Recent commits** (last 5):

### Optional local commands

Commands using `@{upstream}` require an upstream branch to be configured for the current branch.
If these commands fail for other reasons, investigate the underlying git error directly.

```bash
git branch --show-current
git rev-parse --abbrev-ref --symbolic-full-name @{upstream}
git remote | head -n 1 | xargs -I{} git remote show {} | sed -n '/HEAD branch/s/.*: //p'
git status --short --branch
git log -1 --pretty=format:'%h - %an - %ad - %s'
git rev-list --left-right --count @{upstream}...HEAD
git tag --sort=-creatordate | head -n 5
git log --oneline -n 5
```

## 3) Deployment and Maintenance Instructions

### 3.1 Environments

- **Development**:
- **Staging**:
- **Production**:

### 3.2 Deployment

- **Prerequisites**:
- **Build steps**:
- **Configuration / environment variables**:
- **Deployment command or pipeline**:
- **Post-deployment verification**:
- **Rollback procedure**:

### 3.3 Maintenance

- **Monitoring / health checks**:
- **Backup / restore process**:
- **Routine maintenance tasks** (daily/weekly/monthly):
- **Patch / dependency update cadence**:
- **Incident response contact / escalation path**:

## 4) Milestones and Deadlines

| Milestone | Description | Owner | Deadline | Status | Notes |
|---|---|---|---|---|---|
| M1 |  |  | YYYY-MM-DD | Not Started |  |
| M2 |  |  | YYYY-MM-DD | Not Started |  |
| M3 |  |  | YYYY-MM-DD | Not Started |  |

## 5) Risks and Open Items

- **Top risks**:
- **Blocking issues**:
- **Decisions needed**:
