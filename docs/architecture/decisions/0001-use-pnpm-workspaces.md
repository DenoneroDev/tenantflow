# ADR-0001: Use pnpm Workspaces

**Status:** Accepted

## Context

TenantFlow consists of a frontend, backend, background worker and shared packages.

These components require independently defined dependencies while remaining maintainable within one repository.

## Decision

Use pnpm Workspaces to manage applications and shared packages in a single monorepo.

## Alternatives Considered

- Separate Git repositories
- npm Workspaces
- pnpm Workspaces with Turborepo

## Consequences

### Positive
- Shared packages can be developed alongside consuming applications.
- A single lockfile supports reproducible dependency installation.
- Cross-package changes can be reviewed together.

### Negative
- CI must account for multiple packages.
- Package boundaries require discipline.
- Repository tooling may become more complex as the project grows.

## Review Conditions

Reevaluate the build tooling if workspace builds become slow or dependency management becomes difficult.