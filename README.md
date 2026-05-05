# 🎙️ dictationmd

> A standard for defining a speech-to-text correction prompt — so your repo's jargon survives the mic.

## 📄 The Spec

`DICTATION.md` is an optional, repository-level prompt file that corrects transcription text to match repository-specific jargon.

- A speech-enabled editor **SHOULD** automatically detect `DICTATION.md` and use it as a post-processing step after STT.
- Users should be able to choose the LLM model used for correction. `DICTATION.md` should be tuned for small/local models.

## 🤔 Why

Speech-to-text is designed for general-purpose language and commonly mistranscribes repo-specific keywords and acronyms. By providing an LLM-powered mapping and correction layer, transcribed prompts have a much better success rate. It's all about making your code — and your tools — actually understand what you said.

## 🚀 How

You can reuse this dictation prompt generator agentic workflow in your own repo:

- [dictation-prompt.md](https://github.com/github/gh-aw/blob/main/.github/workflows/dictation-prompt.md)

## 🌍 Examples

- [github/gh-aw — DICTATION.md](https://github.com/github/gh-aw/blob/main/DICTATION.md)