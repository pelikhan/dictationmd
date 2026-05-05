---
name: Dictation Instructions
description: Instructions for fixing speech-to-text errors and improving text quality in dictationmd documentation
---

# Dictation Instructions

## Technical Context

dictationmd is a standard for defining repository-level speech-to-text correction prompts. A `DICTATION.md` file provides project-specific vocabulary and correction rules so that LLM-powered editors can post-process speech-to-text output into accurate, repo-aware text.

## Project Glossary

The following project-specific technical terms should be corrected when encountered in speech-to-text input:
DICTATION.md
LLM
README.md
STT
acronyms
agentic
agentic-workflow
auto-detect
correction
dictation
dictationmd
editor
frontmatter
gh-aw
github
github-actions
glossary
jargon
keyword
llm
local-model
markdown
model
pelikhan
post-processing
prompt
repository
small-model
spec
speech-to-text
standard
transcription
workflow
yaml

## Fix Speech-to-Text Errors

When fixing dictated text, correct these common misrecognitions:

### Project Terms
- "dictation M.D." → DICTATION.md
- "dictation markdown" → DICTATION.md
- "read me" → README.md
- "S.T.T." or "S T T" → STT
- "L.L.M." or "L L M" → LLM
- "peli khan" → pelikhan
- "G.H. A.W." → gh-aw
- "front matter" → frontmatter
- "post processing" → post-processing
- "speech to text" → speech-to-text
- "agentic work flow" → agentic-workflow
- "auto detect" → auto-detect
- "small model" → small-model
- "local model" → local-model

### File Formats and Extensions
- "dot M.D." → .md
- "dot Y.A.M.L." or "dot Y M L" → .yaml or .yml

### Technical Patterns
- "A.P.I." → API
- "U.R.L." → URL
- "Y.A.M.L." → YAML

### Common Ambiguities
- "their/there/they're" → use context to determine correct spelling
- "its/it's" → its (possessive), it's (it is)
- "your/you're" → your (possessive), you're (you are)

## Clean Up and Improve Text

Remove filler words and improve clarity:

### Remove These Filler Words
- humm, um, uh, uhh, umm
- you know, like, basically, actually, literally
- kind of, sort of, I mean, I think
- right?, okay?, so yeah, well

### Improve Clarity
1. Remove redundant phrases:
   - "in order to" → "to"
   - "at this point in time" → "now"
   - "due to the fact that" → "because"
   - "in the event that" → "if"

2. Make text more concise:
   - Remove unnecessary qualifiers (very, really, quite)
   - Use active voice instead of passive voice
   - Replace wordy phrases with simpler alternatives

3. Maintain technical accuracy:
   - Keep all technical terms from the glossary
   - Preserve code examples and commands exactly
   - Don't simplify technical concepts

## Guidelines

You do not have enough background information to plan or provide code examples.
- do NOT generate code examples
- do NOT plan steps
- focus on fixing speech-to-text errors and improving text quality
- remove filler words (humm, you know, um, uh, like, basically, actually, etc.)
- improve clarity and make text more professional
- maintain the user's intended meaning
