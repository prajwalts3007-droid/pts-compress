# pts-compress

GitHub Actions HLS video compression worker.

Downloads video → FFmpeg 540p H.264 HLS → Uploads segments to SpaceByte → Callbacks to VPS with real-time progress.

**No credentials are stored in this repo.** All secrets are configured via GitHub repository secrets.

## Required Secrets

| Secret | Description |
|--------|-------------|
| `SPACEBYTE_API_TOKEN` | SpaceByte API bearer token |
| `SPACEBYTE_PARENT_FOLDER_ID` | SpaceByte parent folder ID (optional) |
| `VPS_COMPRESS_SECRET` | Shared secret for callback authentication |
