# AMC12 Study Notes

An Obsidian vault for studying AMC12 through past contests, problem-by-problem
solutions, and topic-based review.

## What Is Included

- `.obsidian/`: Obsidian app, appearance, plugin, graph, hotkey, and theme
  configuration.
- `.agents/skills/`: Local skill sources for working with Obsidian Markdown,
  Bases, Canvas files, the Obsidian CLI, and web page extraction.
- `.claude/skills/` and `.pi/skills/`: Symlinks to the shared skills in
  `.agents/skills/`.
- `skills-lock.json`: Lockfile for the installed Obsidian skills.
- `Problems/`: Exam overviews and individual problem notes.
- `assets/`: Downloaded PDFs and cropped problem or solution images.

## Usage

Open this directory as an Obsidian vault. Each exam is organized as
`Problems/<year>-<part>/`, for example:

```text
Problems/
  2025-A/
    Overview.md
    Q01.md
    Q02.md
assets/
  problems/
    2025-A/
      Q01.png
      2025-AMC12A.pdf
```

`Overview.md` provides the exam source links, a checklist of problems, and an
answer key. Each `Q<number>.md` note contains the problem image, problem
statement, answer, solution, knowledge points, key idea, and common mistakes.

## Notes

Use English filenames and Obsidian Flavored Markdown. For mathematical
notation, use `$...$` for inline LaTeX and `$$...$$` for display LaTeX.
Keep downloaded materials and generated images under `assets/`, using paths
that mirror the related problem notes.
