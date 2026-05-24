At the start of work in this repository, use Smriti for shared agent context:

1. Run `smriti recall "<task or repository topic>" --project video-transcription` when prior decisions may matter.
2. Run `smriti search "<specific term>" --project video-transcription` for exact details.
3. After substantial work, run `smriti ingest codex` so other agents can see the session.

For this machine, the shared memory CLI is `smriti`, backed by `~/.cache/qmd/index.sqlite`.

## Notebook Save Workflow

When changing `whisper_youtube.ipynb`, make the notebook changes directly in this repository, then commit and push them to GitHub. Do not rely on Colab's in-browser GitHub or Drive save popups for persistence, because popup authorization is unreliable in the in-app browser.

After pushing, tell the user to reopen or refresh the Colab notebook from the GitHub URL and run the new/changed cells there. Keep notebook diffs focused: avoid reformatting the whole `.ipynb` JSON when only adding or editing a cell.
