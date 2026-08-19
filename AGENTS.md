# AGENTS.md

This is the GitHub organization-level `.github` repo for Ashfall-Software
(github.com/Ashfall-Software/.github). Its sole purpose is hosting
`profile/README.md`, which renders as the org's homepage on GitHub.
The root `README.md` is a pointer stub — real content edits go in `profile/`.

## Scope gotchas

- The parent directory (`2-repos/ashfall/`) looks like a monorepo but is not.
  Sibling folders (`brews-n-battles`, `cloudflare-workers`,
  `internal.ashfallsoftware.com`, etc.) are independent git repos — never edit
  them from a session rooted here.
- There is no build, lint, test, or CI in this repo. Don't hunt for manifests;
  the only verification is reviewing the rendered markdown on GitHub after push.

## Editing the team list

`profile/README.md` renders members as an HTML `<table>`: one `<td>` per person
(avatar image, username link, role), each with `width="14.28%"`. To add or
change a member, copy an existing `<td>` block and keep the structure and
widths consistent — don't switch to plain Markdown lists.

## Workflow

- Default branch is `main`; history shows content edits committed and pushed
  directly to `main` with short, informal messages — no PRs or feature branches.
