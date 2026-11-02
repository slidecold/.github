# Security policy

## Reporting a vulnerability

Please don't open a public issue for security problems.

- **In an SDK, the CLI or the MCP server:** use **Report a vulnerability** on the repo's Security tab (GitHub private vulnerability reporting).
- **In the SlideCold app or API:** email [support@slidecold.com](mailto:support@slidecold.com) with "SECURITY" in the subject.

Include what you found, how to reproduce it, and the impact you expect. We'll acknowledge your report within 3 business days and keep you updated until it's fixed. Please give us a reasonable chance to fix the issue before you disclose it publicly.

## API keys

If an API key (`cs_...`) has been exposed, delete it right away under **Settings → API Keys** in the dashboard and create a new one. Keys are shown only once and are stored as hashes, so we can't recover them for you.

## Supported versions

Security fixes go into the latest release of each package. Upgrade to get them.

## Verifying releases

Every release is built and published by GitHub Actions with signed build provenance:

- npm: `npm audit signatures`
- PyPI files and CLI binaries: `gh attestation verify <file> --owner slidecold`
