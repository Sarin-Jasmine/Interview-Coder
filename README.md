# Interview Coder

A single-file browser app that codes interview transcripts with the Claude API, using a codebook (with code hierarchy) and your own coded exemplars. Files go only to the Anthropic API with your own key, which stays in the browser tab.

## Use
1. Open `interview-coder.html` (current version, v1.10) in Chrome, Edge or Firefox.
2. Add a transcript (.docx, .odt, .xlsx, .numbers, .csv), the codebook, and one or more coded exemplars.
3. Paste your Anthropic API key, then click **Code transcript**.
4. Optional: set **Consensus runs** (for example 5) for a more repeatable result.

See `docs/01_Collaborator_Guide.docx` for file formats and tips, and `docs/00_Iteration_Report.docx` for the version history.

## Contents
- `interview-coder.html`: current app (v1.10).
- `system_prompt_v1.9.txt`: the shared system prompt.
- `docs/`: collaborator guide.

## Not included
Coded transcripts and below-threshold review lists contain interview text and are not stored here. Keep transcripts anonymized.

## Notes
The model does not accept temperature 0, so runs on identical inputs can differ. Use consensus runs and compare consensus with consensus.
