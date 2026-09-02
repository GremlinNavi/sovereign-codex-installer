# Sovereign Codex Installer

Standalone installer for the Sovereign AI Framework's local Codex + Ollama workflow.

## Current target

- Windows 11
- PowerShell 5.1+
- Git
- Python 3.12
- Ollama
- OpenAI Codex CLI

The installer clones or updates `GremlinNavi/sovereign-ai-framework`, configures local Ollama inference, creates the Python environment, validates the framework, and creates local launchers.

## Install

Review the script before execution, then run:

```powershell
.\Install-SovereignCodex.ps1
```

## Portability

SteamOS/Linux support is planned as a separate installer path rather than pretending the current Windows bootstrap is cross-platform.

## License

Apache License 2.0. See `LICENSE` and `NOTICE`.
