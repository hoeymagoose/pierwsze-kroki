# Pierwsze kroki

Example project README with a sample style guide.

## Style Guide

### General

- Use UTF-8 encoding and LF line endings.
- Indent with 2 spaces (no tabs).
- Keep lines under 100 characters.
- End every file with a single newline.

### Naming

| Item                | Convention         | Example           |
| ------------------- | ------------------ | ----------------- |
| Variables/functions | `camelCase`        | `getUserName`     |
| Classes/types       | `PascalCase`       | `UserProfile`     |
| Constants           | `UPPER_SNAKE_CASE` | `MAX_RETRIES`     |
| Files/directories   | `kebab-case`       | `user-profile.js` |

### Code

- Prefer small, single-purpose functions.
- Avoid abbreviations unless they are widely known (`id`, `url`).
- Comment *why*, not *what*.
- Remove dead code instead of commenting it out.

```js
// Good
const MAX_RETRIES = 3;

function fetchUser(id) {
  return request(`/users/${id}`, { retries: MAX_RETRIES });
}
```

### Commits

- Use the imperative mood: "Add login form", not "Added login form".
- Keep the subject line under 72 characters.
- Separate the subject from the body with a blank line.
- Reference issues where relevant (`Fixes #12`).

### Documentation

- Every public function or module gets a short description.
- Write in plain, concise language.
- Use fenced code blocks with a language tag.
- Use sentence case for headings.

### Pull requests

1. Keep changes focused; one concern per PR.
2. Describe what changed and why.
3. Make sure tests and linters pass before requesting review.
4. Respond to review comments promptly and politely.
