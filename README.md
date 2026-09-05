# OSWAP Codex Installer

Standalone Windows installer for the OSWAP local Codex + Ollama workflow. The source repository remains `sovereign-ai-framework`; that slug is an implementation identifier rather than the installer product name.

## Current target

- Windows 11
- PowerShell 5.1+
- Git
- Python 3.12
- Ollama
- OpenAI Codex CLI

The installer clones or updates `GremlinNavi/sovereign-ai-framework`, configures local Ollama inference, creates the Python environment, validates the framework, and creates local launchers.

## Engineering status

Implemented:

- Windows 11 / PowerShell 5.1+ bootstrap path;
- dependency discovery before installation;
- local Ollama configuration with remote inference disabled by default;
- framework validation and health checks before completion; and
- generated launchers for OSWAP, the Sovereign AI Demonstrator, and local Codex use.

Current boundaries:

- this is a convenience/bootstrap component, not the canonical OSWAP runtime;
- SteamOS/Linux installation remains planned rather than implemented;
- inference runtimes and model weights remain external dependencies; and
- consequential repository publication remains in OSWAP Twin Transport rather than this installer.

## Install

Review the script before execution, then run:

```powershell
.\Install-SovereignCodex.ps1
```

The script filename is retained for compatibility with the current implementation; the repository and component identity are `oswap-codex-installer` / OSWAP Codex Installer.

## Portability

SteamOS/Linux support is planned as a separate installer path rather than pretending the current Windows bootstrap is cross-platform.

## License

Apache License 2.0. See `LICENSE` and `NOTICE`.
