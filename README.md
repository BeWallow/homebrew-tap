# BeWallow Homebrew tap

Homebrew formulas for Déjà tools. Repo name **`homebrew-tap`** → install as **`BeWallow/tap`**.

## Install dsr-verifier-cli

```bash
brew install BeWallow/tap/dsr-verifier-cli
```

## How updates work

On each tagged release of [dsr-verifier-cli](https://github.com/BeWallow/dsr-verifier-cli), CI dispatches a `new-release` event here. The workflow in `.github/workflows/update-formula.yml` bumps `Formula/dsr-verifier-cli.rb` (version + SHA-256 checksums).

## One-time setup (org admin)

1. This repo must exist: `github.com/BeWallow/homebrew-tap`
2. In **dsr-verifier-cli** repo secrets, set `HOMEBREW_TAP_TOKEN` — a GitHub PAT with `repo` access to this repository (classic token or fine-grained).

See [dsr-verifier-cli/docs/HOMEBREW_SETUP.md](https://github.com/BeWallow/dsr-verifier-cli/blob/main/docs/HOMEBREW_SETUP.md) for full steps.
