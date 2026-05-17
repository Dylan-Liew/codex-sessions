# codex-sessions

Small helper script for deleting local Codex session files.

For now, this project is **deletion only**. It lists sessions from a local Codex home, lets you choose one, and requires typing `DELETE` before it removes the matching session file and index entry.

## Usage

```bash
chmod +x codex-session
./codex-session
```

To point it at a specific Codex home:

```bash
CODEX_HOME=/path/to/.codex ./codex-session
```

On WSL, this can be used against a Windows Codex Desktop home by setting `CODEX_HOME` to the mounted Windows `.codex` directory.

## Notes

- Close Codex before deleting sessions manually.
- The script backs up `session_index.jsonl` before editing it.
- No sync, archive, rename, or export features are included yet.
