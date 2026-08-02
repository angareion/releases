# Angareion — Releases

This repository hosts release artifacts for [Angareion](https://angareion.dev):

- **`ang`** — the Angareion CLI
- **`angareion-mcp`** — the Angareion MCP server
- The Claude Code skill pack (`angareion-skills-*.tar.gz`)
- `install.sh` — the zero-install bootstrap script for `ang`

It does not contain source code. Angareion is developed in a private repository;
this repo exists solely so releases have a public home with a clean, versioned
download surface. Binaries are cross-compiled and signed with
[cosign](https://github.com/sigstore/cosign) via GitHub Actions OIDC keyless
signing — see the verification instructions in each release, or
`cmd/ang/README.md` / `cmd/angareion-mcp/README.md` in the Angareion CLI docs.

## Install `ang`

```bash
curl -fsSL https://github.com/angareion/releases/releases/latest/download/install.sh | sh
```

## Everything else

Docs: https://docs.angareion.dev
