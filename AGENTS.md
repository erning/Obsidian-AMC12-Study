# Agent Instructions

This repository is an Obsidian vault. Treat Markdown files as Obsidian Flavored
Markdown and keep vault configuration changes scoped and intentional.

## Repository Layout

- `.obsidian/` stores shared Obsidian settings and the Things theme.
- `Problems/` stores exam notes. Each exam has one directory named
  `<year>-<part>`, containing `Overview.md` and one note per problem.
- `assets/` stores downloaded source files and generated problem or solution
  images. Asset paths should mirror the corresponding problem directory.
- `.agents/skills/` stores the actual skill files.
- `.claude/skills/` and `.pi/skills/` are symlink views into `.agents/skills/`.
- `skills-lock.json` records the installed Obsidian skill set.

## Working Rules

- Preserve symlinks under `.claude/skills/` and `.pi/skills/`.
- Do not commit Obsidian workspace state, caches, `.env` files, dependency
  folders, logs, or OS/editor files.
- Prefer standard Markdown unless Obsidian features such as wikilinks,
  callouts, embeds, properties, Canvas files, or Bases are specifically useful.
- Use wikilinks for vault-internal note links and Markdown links for external
  URLs.
- Use English filenames with consistent names such as `Overview.md`,
  `Q01.md`, and `2025-A`. Keep note content in the language appropriate for
  the study material.
- For Obsidian math, use `$...$` for inline LaTeX and `$$...$$` for
  display LaTeX. Use local image embeds when Markdown or LaTeX cannot clearly
  represent a problem.
- Keep generated docs short, practical, and readable in Obsidian.

## Git

- Use Conventional Commits.
- Commit messages must be in English and ASCII.
- Stage only files relevant to the requested change.
