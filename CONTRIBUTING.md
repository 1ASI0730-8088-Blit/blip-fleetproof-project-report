# Contribution Guide

## Branches

- `main`: released report versions only.
- `develop`: integrated work for next delivery.
- `docs/<scope>`: documentation work.
- `feature/usXXX-<short-name>`: software feature linked to one User Story.
- `release/vX.Y.Z`: release stabilization.
- `hotfix/<short-name>`: urgent correction over released version.

## Commit Messages

Use Conventional Commits:

- `docs: add lean ux problem statement`
- `docs: update competitive analysis`
- `feat: implement landing page hero`
- `fix: correct landing page accessibility labels`
- `chore: organize report assets`

## Pull Requests

Each Pull Request must include:

- Related section or User Story.
- Screenshots or evidence when applicable.
- Checklist against rubric criteria.
- Reviewer approval before merge.

## Markdown Rules

- Use English for product UI terms when required by the course.
- Use correct Spanish engineering terms: requisito, aplicación, despliegue, pruebas.
- Review the official terminology from Annex E before every Pull Request.
- Keep evidence as links plus screenshots in `assets/screenshots/`.

## Rubric Review Before Merge

Before merging any Pull Request, the reviewer must verify:

- The edited content follows the official report structure.
- The text uses correct software engineering terminology.
- The evidence is traceable through branch, commit, Pull Request and merge.
- Screenshots and links match the section where they are cited.
- The content includes no informal class slang in formal report sections.
