# adze-dev — Agent Instructions

This repository is the contributor/dev integration repo for Adze.

## Routing

- External public contributions belong in `EffortlessMetrics/adze`.
- Swarm-generated work belongs in `EffortlessMetrics/adze-swarm`.
- Do not target this repo for swarm PRs unless explicitly instructed.

## Promotion model

Promotion and sync between repos happens through Git branches and PRs, not copied file snapshots.

- `adze-swarm` → `adze`: explicit promotion PRs from `swarm/` or `promote/` branches.
- `adze` (external PRs) → `adze-dev` / `adze-swarm`: sync PRs to pull public history back into integration trunks.

## CI

This repo is **not** wired to the `em-ci-small` self-hosted runner group. CI here, when added, should run on GitHub-hosted runners only.
