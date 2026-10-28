# Lernex Homebrew tap

```bash
brew install lernex/tap/lernex
```

This installs [Lernex](https://github.com/lernex/lernex-engine), the inference engine for the Metis models, on a Mac
with Apple silicon and macOS 14 or newer. It runs on the Mac's GPU through Metal.

```bash
lernex run praxis      # downloads the model, then chats in the terminal
lernex serve praxis    # an OpenAI-compatible API on port 8080
lernex doctor praxis   # every format, what fits on this Mac and the speed to expect
```

`brew upgrade lernex` updates it. Each release moves `Formula/lernex.rb` to its tarball with
`packaging/homebrew-tap/bump-formula.sh` in the engine's repository.
