# Homebrew tap

Formulae for my projects.

## Install

```bash
brew install nub235/tap/s1-mini-engine
```

### [`s1-mini-engine`](https://github.com/nub235/s1-mini-engine)

A tiny, self-contained Swift engine for running [Superwhisper
S1-mini](https://huggingface.co/superwhisper/s1-mini) locally to clean up
speech-to-text transcripts. This formula installs the prebuilt binary; there is
no build step and no Swift toolchain required.

Requires an Apple Silicon Mac on macOS 14 (Sonoma) or newer.

The model weights are **not** bundled — they are ~495 MB and the engine works
fine without them until you use it. Fetch them once:

```bash
s1-mini-engine pull
```

Then:

```bash
s1-mini-engine "um so uh the deploy failed again"
```
