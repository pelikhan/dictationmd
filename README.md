# dictationmd
A standard to define a speech to text correcting prompt.

## The spec

DICTATION.md is an optional repository level prompt file that corrects transcriltion text to repository jargon.

- An editor speech enabled SHOULD automatically detect DICTATIOM.md and use it as a post processing step of STT.
- The user should be able to choose the LLM model to apply corrextion. DICTATION.md should be tuned for small/local models.

## Why

STT is designed for general purpose language and commonly mistranscribes repo specifix keywords and acronyms. By proving an LLM powered mapping/correction, the transcribed prompts have much better success rate. It's all aboit making grep happy.

## Examples

- github/gh-aw https://github.com/github/gh-aw/blob/main/DICTATION.md