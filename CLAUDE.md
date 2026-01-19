# CLAUDE.md

## Project

**pragma-docs**: Documentation for the Pragmatiks platform, hosted on [docs.pragmatiks.io](https://docs.pragmatiks.io).

## Deployment

Deployed via **Mintlify** - push to `main` auto-deploys.

**Preview**: Mintlify provides preview URLs for PRs.

**Config**: `docs.json` defines navigation, theme, and settings.

---

# Mintlify documentation

## CONFIDENTIAL - DO NOT PUBLISH

**The following internal implementation details are CONFIDENTIAL and must NEVER appear in documentation:**

| Category | Forbidden Terms |
|----------|-----------------|
| Message queue | NATS, JetStream, message broker, event streaming |
| Database | SurrealDB, graph database internals |
| Scaling | KEDA, auto-scaling implementation, consumer groups |
| Build system | BuildKit, tarball creation, container build process |
| Architecture | Internal service communication, queue depths, retry mechanics |

**What TO document:**
- Command syntax and options
- User-facing workflows
- Resource YAML structure
- High-level concepts (what users need to know)

**What NOT to document:**
- How the system works internally
- Internal URLs, ports, paths
- Authentication token storage locations
- Provider deployment internals
- Message delivery mechanics

If unsure whether something is confidential, ASK before including it.

---

## Working relationship
- You can push back on ideas-this can lead to better documentation. Cite sources and explain your reasoning when you do so
- ALWAYS ask for clarification rather than making assumptions
- NEVER lie, guess, or make up information

## Project context
- Format: MDX files with YAML frontmatter
- Config: docs.json for navigation, theme, settings
- Components: Mintlify components

## Content strategy
- Document just enough for user success - not too much, not too little
- Prioritize accuracy and usability of information
- Make content evergreen when possible
- Search for existing information before adding new content. Avoid duplication unless it is done for a strategic reason
- Check existing patterns for consistency
- Start by making the smallest reasonable changes

## Frontmatter requirements for pages
- title: Clear, descriptive page title
- description: Concise summary for SEO/navigation

## Writing standards
- Second-person voice ("you")
- Prerequisites at start of procedural content
- Test all code examples before publishing
- Match style and formatting of existing pages
- Include both basic and advanced use cases
- Language tags on all code blocks
- Alt text on all images
- Relative paths for internal links

## Git workflow
- NEVER use --no-verify when committing
- Ask how to handle uncommitted changes before starting
- Create a new branch when no clear branch exists for changes
- Commit frequently throughout development
- NEVER skip or disable pre-commit hooks

## Do not
- Skip frontmatter on any MDX file
- Use absolute URLs for internal links
- Include untested code examples
- Make assumptions - always ask for clarification
