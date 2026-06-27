# Deployment Checklist

## Before Build

- Product acceptance criteria reviewed.
- Design quality gates passed.
- Visual QA passed.
- Required tests passed.
- Environment variables documented.

## Build

- Run lint.
- Run type check when applicable.
- Run tests.
- Run production build.

## Preview

- Deploy preview environment.
- Inspect primary routes.
- Re-run visual QA on preview URL.

## Release

- Confirm rollback path.
- Tag or record release version.
- Deploy production.
- Smoke test production.

## After Release

- Monitor errors.
- Monitor performance.
- Check analytics for primary workflow.
- Log follow-up improvements.

