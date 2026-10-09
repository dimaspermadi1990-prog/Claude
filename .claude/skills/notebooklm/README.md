# NotebookLM skill (vendored)

`SKILL.md` and `LICENSE` are copied unchanged from
[teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) at release
`v0.8.4` (commit `bff7c66`), MIT licensed.

Claude Code picks it up automatically from `.claude/skills/notebooklm/` when
working in this repo; ask it to do something with NotebookLM / Gemini Notebook.

## One-time setup (on your machine)

```bash
uv tool install "notebooklm-py[browser]"   # or: pipx install / pip install
notebooklm login                            # opens a browser to sign in to Google
notebooklm auth check --test --json         # expect "status": "ok"
```

Credentials live in `~/.notebooklm/` and are bearer tokens: never commit them.
For headless/CI use, see the "Setup and Authentication" section of `SKILL.md`.

## Updating

```bash
notebooklm skill install --scope project --target claude --force
```

or re-copy `SKILL.md` from a newer release tag.
