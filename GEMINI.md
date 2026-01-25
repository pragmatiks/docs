# Pragma Docs Context

## Overview
`pragma-docs` contains the official documentation for the Pragmatiks platform, built with **Mintlify**.

## Architecture
*   **Framework**: Mintlify (MDX-based).
*   **Config**: `docs.json` controls navigation, theme, and settings.
*   **Content**: MDX files organized by topic (e.g., `cli/`, `sdk/`, `concepts/`).

## Development

### Key Commands
Run these from the `pragma-docs` directory.

*   `mintlify dev`: Start the local development server (usually on http://localhost:3000).

### Structure
*   `api-reference/`: OpenAPI specs and API docs.
*   `building-providers/`: Guide for SDK users.
*   `cli/` & `sdk/`: Reference documentation.
*   `assets/`: Images and static resources.

## Conventions
*   **Frontmatter**: Every MDX file MUST have `title` and `description`.
*   **Links**: Use relative paths for internal links.
*   **Components**: Use Mintlify's built-in components (e.g., `<Card>`, `<CodeGroup>`) for better UX.
