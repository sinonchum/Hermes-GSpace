# Privacy Policy for Hermes GSpace

**Effective Date:** October 7, 2026

## Introduction

Hermes GSpace is an open-source skill that enables the Hermes AI agent to interact with Google Workspace services (Gmail, Google Drive, Google Docs, Google Sheets, and Google Calendar) through the official `gws` CLI provided by Google. This privacy policy explains how data is handled when you use this integration.

## Data We Access

This integration accesses only the Google Workspace data you explicitly authorize through Google's OAuth consent screen. The specific data depends on the scopes you grant:

- **Google Drive**: Files created by or explicitly opened to the application (scope: `drive.file`)
- **Gmail**: Messages for reading and sending (scopes: `gmail.readonly`, `gmail.send`)
- **Google Docs & Sheets**: Documents you choose to create, read, or edit
- **Google Calendar**: Calendar events for reading (read-only by default)

## Data We Do NOT Access

We do **not** request or store:
- Your Google account password
- Broad access to all files in your Drive
- Ability to delete emails, Drive files, or Calendar events
- Admin-level access to Google Workspace organization data

## How Data Is Used

- All operations are performed **locally** on your machine through the `gws` CLI
- Data is used solely to fulfill the commands you issue to the Hermes agent
- No user data is transmitted to third-party servers beyond Google's own APIs
- No data is used for advertising, profiling, or model training

## Data Storage

- OAuth tokens are encrypted and stored locally by the `gws` CLI in your user's configuration directory (typically `~/.config/gws/`)
- The Hermes GSpace skill itself does not store your Google data or credentials
- You can revoke access at any time through your [Google Account permissions page](https://myaccount.google.com/permissions)

## Security Practices

- We follow the principle of **least privilege**: only the minimum necessary OAuth scopes are requested
- We prohibit destructive operations (delete, trash, permanent removal) by policy
- OAuth credentials are never logged, printed, or shared in chat transcripts

## Third-Party Services

This integration relies on:
- **Google Workspace APIs** (subject to [Google's Privacy Policy](https://policies.google.com/privacy))
- **gws CLI** by Google Workspace (open-source, not an officially supported Google product)

## Open Source

This skill is open-source. You can inspect the code, suggest changes, or fork it for your own use:
- Repository: https://github.com/sinonchum/Hermes-GSpace

## Contact

For questions or concerns about this privacy policy or the Hermes GSpace integration, please open an issue in the GitHub repository.

## Changes to This Policy

We may update this privacy policy from time to time. Any changes will be posted to the GitHub repository with an updated effective date.
