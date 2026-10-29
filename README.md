# Lernex Homebrew tap

```bash
brew trust --formula lernex/tap/dromos
brew install lernex/tap/dromos
```

Homebrew 7 loads a formula from a third-party tap only after you trust it, so the first line trusts this one
formula and nothing else in the tap.

This installs [Dromos](https://github.com/lernex/dromos), Lernex's inference engine for the Metis models, on a Mac
with Apple silicon and macOS 14 or newer. It runs on the Mac's GPU through Metal.

```bash
dromos run praxis      # downloads the model, then chats in the terminal
dromos serve praxis    # an OpenAI-compatible API on port 8080
dromos doctor praxis   # every format, what fits on this Mac and the speed to expect
```

`brew upgrade dromos` updates it. Each release moves `Formula/dromos.rb` to its tarball with
`packaging/homebrew-tap/bump-formula.sh` in the engine's repository.
