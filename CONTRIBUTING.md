# Contributing to TenantFlow

TenantFlow is an independently developed portfolio project
following professional software engineering practices.

## Development Workflow

1. Create or select a GitHub issue.
2. Define the scope and acceptance criteria.
3. Create a branch from the latest `main`.
4. Implement the change.
5. Add or update relevant tests.
6. Run applicable quality checks.
7. Open a pull request.
8. Review the changes and resolve issues.
9. Merge after all required checks pass.

## Branch Naming

Use the following conventions:

- `feat/<issue>-description`
- `fix/<issue>-description`
- `docs/<issue>-description`
- `test/<issue>-description`
- `refactor/<issue>-description`
- `chore/<issue>-description`

Example:

`feat/12-customer-creation`

## Commit Messages

Follow Conventional Commits:

`type(scope): description`

Examples:

- `feat(customers): add customer creation endpoint`
- `fix(auth): reject expired sessions`
- `test(orders): cover transaction rollback`
- `docs: document repository workflow`

Commits should represent coherent, reviewable changes.

## Pull Requests

Each pull request should:

- Reference its GitHub issue when applicable
- Explain the motivation and implementation
- Document relevant test results
- Highlight security or migration implications
- Remain reasonably small and focused

## Definition of Done

A change is complete when:

- Acceptance criteria are satisfied
- Relevant tests pass
- Type checking and linting pass
- Documentation is updated where necessary
- Security implications are considered
- The pull request has been reviewed
- Required CI checks pass

## Code Review

The project is currently maintained by a single developer.

Every pull request receives a documented self-review.
External reviews are welcome but are not represented
as completed unless they actually occurred.
