# Angareion — Releases

This repository hosts release artifacts for [Angareion](https://angareion.dev):

- **`ang`** — the Angareion CLI
- **`angareion-mcp`** — the Angareion MCP server
- The skill packs (`angareion-skills-*`) for Claude Code, Claude, Perplexity and Joule Work Desktop
- The Joule local proxy (`angareion-joule-local-proxy-*.zip`), for workspaces that cannot add the remote connector
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

## Joule Work Desktop

Each `ang-v*` release has two separate Joule downloads:

- `angareion-skills-joule-vX.Y.Z.zip`: the Angareion skill. Import it in Joule under
  **Extensions → Skills → Import**; do not unzip it.
- `angareion-joule-local-proxy-vX.Y.Z.zip`: the local proxy, for Joule workspaces that cannot add
  the remote connector. It needs Node.js 18 or newer; unzip it and follow the `README.md` inside.

Open the [newest `ang-v*` release](https://github.com/angareion/releases/releases?q=ang-v) and
download them from **Assets**. Step-by-step guide:
https://docs.angareion.dev/connect#joule-local-proxy

## Everything else

Docs: https://docs.angareion.dev
