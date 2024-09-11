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
fix(token): resolve token expiry issue
```

### `feat`
Used for adding new features to the codebase.

**Example:**
```scss
feat(map): add search functionality to the map component
```

### `build`
Changes that affect the build system or external dependencies, like npm, Gradle, or gulp tasks.

**Example:**
```scss
build(deps): update dependency versions
```

### `chore`
Routine tasks and maintenance activities that do not modify the source code.

**Example:**
```scss
chore: update .gitignore to exclude IDE files
```

### `ci`
Changes related to Continuous Integration (CI) configurations and scripts.

**Example:**
```scss
ci: update GitHub Actions for testing
```

### `docs`
Updates to documentation (README, code comments, etc.).

**Example:**
```scss
docs(readme): clarify setup instructions
```

### `style`
Code formatting changes, such as whitespace or semicolon adjustments, that do not affect functionality.

**Example:**
```scss
style: format code according to linter rules
```

### `refactor`
Code refactoring changes that neither fix a bug nor add a feature but improve code readability or structure.

**Example:**
```scss
refactor(login): simplify user validation logic
```

### `test`
Changes or additions to the test suite (unit tests, integration tests, etc.).

**Example:**
```scss
test: add unit tests for login service
```


## Optional Fields

### **`[optional scope]`**
The optional scope is a noun that describes what part of the code is being changed. Use it to provide clarity on which module, component, or system is impacted by the commit.

**Example:**
```scss
feat(auth): add JWT validation logic
```

### **`<description>`**
The description is a short, imperative message that explains the intent of the change. Avoid using past tense; instead, focus on what the commit does, as if giving a command:

- Use "add" instead of "added" or "adds."
- Use "fix" instead of "fixed" or "fixes."

**Example:**
```scss
fix(auth): resolve token expiry issue
```

### **`[optional body]`**
The body is free-form text to explain the purpose behind the changes. This is where you can give more detailed information if necessary.

**Example:**
```scss
refactor(auth): simplify token handling

Updated token validation to reduce code duplication and improve error handling logic.
```

### **`[optional footer(s)]`**
The footer contains metadata, such as issue references, links, or co-authorship information. Common tokens include:

- **`Resolves`** – Links the commit to an issue that is being resolved.
- **`Co-authorship`** – Mention the authors involved in the commit.

**Examples:**

**Resolves an issue:**
```scss
fix(auth): resolve token expiry issue

Ensures that tokens are refreshed properly when nearing expiration.

Resolves #123
```

**Resolves an issue:**
```scss
feat(map): add route visualization

Users can now see the path to a destination.

Development-Method: Pair Programming
With: James
```

## Example Commit Messages

### Simple commit with description:
```scss
fix(auth): resolve token expiry issue
```

### Commit with description and scope:
```scss
feat(map): add search functionality to the map component
```

### Commit with body and footer:
```scss
refactor(login): simplify user validation logic

Simplified the user validation logic to reduce code complexity and improve performance.

Resolves #45
```

This structure ensures consistency in commit messages, making it easier to understand project history and collaborate with others effectively.


