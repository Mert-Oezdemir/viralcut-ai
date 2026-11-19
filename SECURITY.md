# Security and privacy

This is a local-first development prototype. **Do not deploy the API on a public interface** without authentication, quotas and an additional security audit. Keep it bound to `127.0.0.1`.

- Never commit `.env`, API keys, tokens, downloaded videos, generated Shorts, comment exports, local databases or the `workspace/` directory.
- `.env.example` contains placeholder variable names only. Put real secrets in your private `.env` file, which is ignored by Git.
- Do not make GitHub Actions print environment variables or publish test fixtures containing personal data.
- If using Gemini, uploaded video data may leave the machine; the offline analysis and FFmpeg paths do not need remote model access.
- The YouTube URL inspection workflow is not permission to download, edit or redistribute someone else's work.
- Videos are not automatically uploaded to YouTube.
- Dependencies and optional download integrations should be reviewed and kept updated before deployment.

If a secret is accidentally committed, **revoke/rotate the credential immediately**. Deleting it in a later commit does not remove it from git history.
