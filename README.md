# 🎙️ dictationmd

> A standard for defining a speech-to-text correction prompt — so your repo's jargon survives the mic.

## 📄 The Spec

`DICTATION.md` is an optional, repository-level prompt file that corrects transcription text to match repository-specific jargon.

- A speech-enabled editor **SHOULD** automatically detect `DICTATION.md` and use it as a post-processing step after STT.
- A speech-enabled editor **MUST** ask the user for permission before using `DICTATION.md` for the first time.
- Users should be able to choose the LLM model used for correction. `DICTATION.md` should be tuned for small/local models.

## 📋 Frontmatter

`DICTATION.md` supports optional YAML frontmatter fields:

| Field | Type | Description |
|-------|------|-------------|
| `description` | string | A short description of the dictation prompt, shown to the user when asking for permission. |
| `model` | string | The preferred LLM model identifier to use for correction (e.g. `gpt-4o-mini`, `phi3`). The editor **MAY** use this as a default, but users **SHOULD** be able to override it. |

Example:

```markdown
---
description: Corrects speech-to-text for the dictationmd project vocabulary.
model: gpt-4o-mini
---
```

## 🤔 Why

Speech-to-text is designed for general-purpose language and commonly mistranscribes repo-specific keywords and acronyms. By providing an LLM-powered mapping and correction layer, transcribed prompts have a much better success rate. It's all about making your code — and your tools — actually understand what you said.

## 🚀 How

You can reuse this dictation prompt generator agentic workflow in your own repo:

- [dictation-prompt.md](https://github.com/github/gh-aw/blob/main/.github/workflows/dictation-prompt.md)

## 🌍 Examples

- [github/gh-aw — DICTATION.md](https://github.com/github/gh-aw/blob/main/DICTATION.md)