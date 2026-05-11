# Obsidian Setup

## Vault
Open `/root/.openclaw/workspace` as an Obsidian vault.

## Useful plugins
- Dataview
- Templater

## Suggested daily note template
```md
# <% tp.date.now("YYYY-MM-DD") %>

## Session Log

## Decisions Made

## Things to Remember
```

## Simple Dataview query
```dataview
LIST FROM "memory" SORT file.name DESC LIMIT 7
```

## Notes
- Graph View works best when notes use `[[wiki-links]]`.
- QMD is not installed here yet, so semantic search is still a future step.
