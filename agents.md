# Project Information Template (for local codebase analysis)

Use this template to generate a project status document from a local software repository.

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

```bash
git branch --show-current
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
