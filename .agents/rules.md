# Agent Rules — Tibetan Calendar Wiki

High-signal non-negotiables for agents working on the Tibetan Calendar Wiki.

## Core Rules

- **Pure data repo**: only `raw/` and `wiki/` content. Do not add runtime code,
  build scripts, or tool configs except for validation/secret-scanning wiring.
- **No secrets**: never commit credentials, API keys, or per-user paths.
- **Markdown style**: keep all `.md` under 100 characters per line and pass
  `paniolo scan --fail-on warn .`.
- **Source of truth**: `raw/` snapshots are canonical evidence; `wiki/` pages
  must cite them and pass `paniolo wiki` validation.
