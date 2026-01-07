# Repository Guidelines

## Project Structure & Module Organization
- `index.html` is the single-page site with semantic sections (header, about, footer).
- `style.css` contains all styling, including responsive rules and dark mode overrides.
- `assets/` holds static assets like `assets/headshot.jpg`.
- `favicon.svg` provides the favicon; `CNAME` configures the GitHub Pages domain.
- `README.md` and `CLAUDE.md` document project context and workflow notes.

## Build, Test, and Development Commands
This is a static site with no build system.
- Open `index.html` directly in a browser for local preview.
- Optional local server:
  - `python3 -m http.server` (then visit `http://localhost:8000`).

## Coding Style & Naming Conventions
- HTML: keep semantic structure and match existing indentation within the file.
- CSS: 4-space indentation, lower-case hex colors, and class names in kebab-case (e.g., `.header-text`).
- Keep dark mode overrides at the end of `style.css` under `@media (prefers-color-scheme: dark)` to ensure proper overrides.
- Maintain the minimalist, monochrome visual style and IBM Plex Mono typography.

## Testing Guidelines
No automated tests are configured.
- Manually verify in a browser:
  - Layout at desktop and at `<= 600px` width.
  - Dark mode in a system with `prefers-color-scheme: dark`.
  - Links and images load correctly.

## Commit & Pull Request Guidelines
- Commit messages are short, imperative, and descriptive (e.g., "Add favicon with LSF initials", "Update index.html").
- Keep commits focused on a single change or theme.
- PRs should include:
  - A brief summary of changes and rationale.
  - Screenshots for any visual or layout updates.
  - Notes on any content or external link changes.

## Deployment & Configuration
- Pushing to `main` deploys via GitHub Pages to `https://leonf.me`.
- Do not remove or rename `CNAME` unless you intend to change the custom domain.
