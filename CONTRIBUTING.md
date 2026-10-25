# Contributing

## Branches
- `main`: production code. Never push directly.
- `develop`: integration branch (Test). All PRs target `develop`.
- `feature/INSD-<no>-<short-name>`: new work, created from latest `develop`.
- `fix/INSD-<no>-<short-name>`: bug fix, created from latest `develop`.
- `release/vX.Y.Z`: frozen release candidate (Pilot).
- `hotfix/INSD-<no>-<short-name>`: emergency fix, created from `main`.

## Commits
- One clear change per commit.
- Start the message with the ticket number: `INSD-12: add fee receipt page`.

## Pull requests
1. Branch from the latest `develop`.
2. Push the branch and open a PR into `develop` (never `main`).
3. Fill in the PR template completely.
4. CI must be green and a reviewer must approve.
5. You cannot approve your own PR.
6. After merge, delete the feature branch.

## Releases
- Cut `release/vX.Y.Z` from the QA-approved `develop` commit.
- Only fixes go into a release branch, no new features.
- Version numbers: X = breaking change, Y = new feature, Z = fix only.
