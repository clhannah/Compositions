# Compositions — ARC Project

## Where the work lives

Source material is **not in this repo**. It lives in Dropbox under `/Compositions`,
reached through the Dropbox MCP tools. This repo holds project scaffolding, notes,
and any scripts — the manuscripts and working documents stay in Dropbox.

Namespace path prefix for MCP calls:

```
ns:463631132//compositions/
```

Use the `ns:` form returned by `list_folder`/`search` for follow-on calls; the
display form (`/Compositions/...`) is case-insensitive and also accepted.

Relevant tools: `mcp__Dropbox__list_folder`, `mcp__Dropbox__search`,
`mcp__Dropbox__fetch` (read text, 5 MiB cap), `mcp__Dropbox__create_file`,
`mcp__Dropbox__create_folder`, `mcp__Dropbox__file_preview`.

Note: `list_folder` defaults to **recursive** — pass `recursive: false` to browse
one level.

## Dropbox layout (top level of /Compositions)

- `ARCs.docx` — ARC working document (currently empty)
- `Proofing/` — copy-editing workflow; has its own `CLAUDE.md`
- `Creatives/` — has its own `CLAUDE.md`
- `Proposals/`, `Submissions/`, `where are the proposals/`
- Manuscript folders: `Overseers`, `Interregnum`, `Timeless War`,
  `Duchess of Eastmarck`, `Dalliance`, `White Queen`, `Hearthside Series`,
  `A Walk in the Garden`, `Craniax`
- `Comprehensive To Do's.docx`, `Manuscript_Comparative_Analysis_April2026.docx`
- `fonts/`, `.claude/`

`/Compositions/CLAUDE.md` in Dropbox is a pointer file: it defers to
`Proofing/CLAUDE.md` and `Creatives/CLAUDE.md`. Read the relevant one before
doing writing or copy-editing work.

## Conventions

- Dropbox cannot overwrite an existing file in place — `create_file` makes new
  files only. To revise a document, write a new version rather than expecting an
  edit, and confirm before `move`/`delete`.
- Don't copy manuscript text into this repo unless asked.
- Work on the branch named in the session brief; commit and push there.

## Open

- ARC platform decisions (Booksprout, BookSirens, and others discussed in an
  earlier session) are **not recorded anywhere reachable**. Prior session
  transcripts are not readable from here and `ARCs.docx` is empty. Capture those
  notes here or in `ARCs.docx` before building on them.
