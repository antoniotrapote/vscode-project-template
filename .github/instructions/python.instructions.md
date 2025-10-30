---
applyTo: "**/*.py"
description: "Coding standards for all Python source files"
---

# Project coding standards for Python

- **Style**
  - Follow the PEP 8 style guide.
  - Use `snake_case` for variables and functions.
  - Use `PascalCase` for class names.
  - Keep line length at 79 characters for code (PEP 8 standard), or up to 99 characters for compatibility.

- **Readability**
  - Always prioritize clarity and simplicity over cleverness.
  - Write self-explanatory code and avoid unnecessary complexity.

- **Documentation**
  - Add docstrings to all functions, classes, and modules using triple quotes.
  - Include docstrings for both public and private functions to aid code understanding.
  - Write comments only for non-obvious parts of the code.
  - Keep docstrings concise but descriptive.

- **Functions**
  - Use descriptive names.
  - Always include type hints for parameters and return values.
  - Keep functions small and focused on a single task.

- **Testing**
  - When writing new functions, add simple unit tests with `pytest`.
  - Tests should cover typical cases and edge cases.

- **Dependencies**
  - Prefer Python standard library over external packages, unless otherwise required.
  - When suggesting an external package, explain why it's necessary.
  - Keep the `requirements.txt` file up to date with pinned versions when appropriate.

- **Code Quality**
  - Avoid global variables and side effects.
  - Write small, reusable, and pure functions whenever possible.
  - Ensure code is efficient and avoids unnecessary computations.
  - Prefer clarity over brevity.

- **Security**
  - Avoid hardcoding sensitive information like API keys or passwords.
  - Follow best practices for handling user input to prevent security vulnerabilities.
  - Validate and sanitize external input appropriately.