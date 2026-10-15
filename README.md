# agy-delegate

A Claude Code skill: delegate a bounded coding task to the Google Antigravity CLI (`agy`) as a background implementer, then review its diff and land it yourself.

## Install

```bash
npx skills add Nick-800/agy-delegate
```

## Requirements

- `agy` CLI installed and authenticated
- Node.js and git

## Note on permissions

Headless `agy` may auto-deny file writes. The relay supports `--dangerously-skip-permissions`; only use it if you understand and accept that agy then writes without prompting. agy never commits; you review the diff first.
