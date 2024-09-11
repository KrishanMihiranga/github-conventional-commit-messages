# Conventional Commits Guide

This guide outlines the **Conventional Commits** specification to help structure your commit messages. This makes them more readable and provides better context for others reviewing the project history.

### Commit Message Structure

A conventional commit message follows this pattern:

```text
<type>[optional scope]: <description>
[optional body]
[optional footer(s)]
```

#### Elements:

1. **`<type>`** – Specifies the type of change you're making. Examples include fix, feat, build, etc.
2. **`[optional scope]`** – Provides additional context to specify what part of the project is affected. This is optional but should use nouns to clarify the area of the code being modified.
3. **`<description>`** – A brief, imperative sentence describing the change
4. **`[optional body]`** – An optional free-form explanation of the changes made.
5. **`[optional footer(s)]`** – Used for metadata, such as issue references, or co-authors. Can be used for any additional information, such as issue resolution or coding practices.


## Commit Types

### `fix`
Used for bug fixes. These changes address issues or errors in the code.

**Example:**
```scss
fix: resolve token expiry issue
```

### `feat`
Used for adding new features to the codebase.

***Example:**
```scss
feat(map): add search functionality to the map component
```

### `build`
Changes that affect the build system or external dependencies, like npm, Gradle, or gulp tasks.

Example:

build(deps): update dependency versions


### `chore`
Routine tasks and maintenance activities that do not modify the source code.

Example:

chore: update .gitignore to exclude IDE files


### `ci`
Changes related to Continuous Integration (CI) configurations and scripts.

Example:

ci: update GitHub Actions for testing


### `docs`
Updates to documentation (README, code comments, etc.).

Example:

docs(readme): clarify setup instructions


### `style`
Code formatting changes, such as whitespace or semicolon adjustments, that do not affect functionality.

Example:

style: format code according to linter rules


### `refactor`
Code refactoring changes that neither fix a bug nor add a feature but improve code readability or structure.

Example:

refactor(login): simplify user validation logic


### `test`
Changes or additions to the test suite (unit tests, integration tests, etc.).

Example:

test: add unit tests for login service
