# Data Refinery Project

This project tracks 30,000 development phases for data refinery implementation.

## Branching Strategy

- `main` (formerly master): Production-ready releases
- `develop`: Integration branch for ongoing development
- `feature/phase-X`: Feature branches for individual phases (e.g., feature/phase-1, feature/phase-2)
- `hotfix/*`: Branches for critical fixes to main

### Workflow

1. Create feature branches from `develop` for each phase: `git checkout -b feature/phase-1`
2. Develop and commit changes
3. Push feature branch: `git push -u origin feature/phase-1`
4. Create pull request to merge into `develop`
5. After testing, merge to `main` for releases
6. Use tags for phase milestones: `git tag phase-1 && git push --tags`

### Phase Tracking

Each of the 30,000 phases will be tracked via GitHub issues, with corresponding feature branches.

## Setup

- Python 3.11+
- Use Black for formatting
- Use Ruff for linting
- Pre-commit hooks enforce standards
