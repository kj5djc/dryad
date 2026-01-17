# Copilot Instructions

## Project Overview

DRYAD.js is a JavaScript implementation of the DRYAD Authentication System — a military-style code sheet generator used for challenge-response authentication.

## Commit Convention

This project uses **Conventional Commits**. All commit messages must follow this format:

```
<type>(<scope>): <description>
```

### Commit Types

| Type | Description |
|------|-------------|
| `feat` | A new feature or functionality |
| `fix` | A bug fix |
| `docs` | Documentation only changes |
| `style` | Changes that do not affect code meaning (whitespace, formatting, semicolons) |
| `refactor` | Code change that neither fixes a bug nor adds a feature |
| `perf` | Code change that improves performance |
| `test` | Adding or correcting tests |
| `build` | Changes to build system or external dependencies |
| `ci` | Changes to CI configuration files and scripts |
| `chore` | Other changes that don't modify src or test files |
| `revert` | Reverts a previous commit |

### Examples

```
feat: add PDF export functionality
fix: correct grid alignment on mobile devices
docs: update README with usage instructions
style: format code with prettier
refactor: extract authentication logic into separate module
perf: optimize random code generation
test: add unit tests for grid generation
build: update dependencies
chore: update .gitignore
```

### Breaking Changes

For breaking changes, add `!` after the type or include `BREAKING CHANGE:` in the footer:

```
feat!: redesign authentication grid format
```
