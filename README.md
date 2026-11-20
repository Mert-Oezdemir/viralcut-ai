# ViralCut AI

Local-first AI-assisted video clipping project for vertical Shorts.

> **Source import status:** The public repository is being prepared. The application's Python backend, browser UI and test suite are not yet present in this repository. Do not assume it can run from this repository until those files are imported and verified.

## Planned / packaged capabilities

- Analyze uploaded, rights-cleared video files and suggest vertical clips.
- Optional Gemini API-assisted scene and speech understanding.
- Optional YouTube Data API-based topic discovery and timestamped-comment signals.
- Local FFmpeg rendering and optional Whisper speech-to-text.
- Browser-based clip review, cuts, and export.

The packaged v0.2 source contains an experimental implementation. Its automated clip scores are heuristic and do not guarantee a viral result.

## Safety and privacy

Do not commit local media, exported Shorts, API credentials or private configuration. Use the placeholder `.env.example` as a guide and keep real keys in `.env`. The `.gitignore` excludes local secrets, runtime files and media.

For restrictions and usage notes, see [SECURITY.md](SECURITY.md).

## Usage rights

Analyze and edit only video media you own or have permission to process. Public availability of a YouTube URL does not grant downloading or redistribution rights.

## Planned local requirements

Python 3.11+, FFmpeg, the packages in `requirements.txt`, and optional Gemini / YouTube API credentials. Full installation commands will be documented when the source is imported.
