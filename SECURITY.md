# Security and privacy

## Never commit

- API keys or provider credentials.
- JWT/signing secrets.
- Owner/admin passwords or access tokens.
- `.env` files containing real values.
- Production database dumps or user records.
- Personal information that is not required for the public project.

Use example placeholders in documentation. Keep real credentials in private hosting environment settings.

## Reporting

For a suspected vulnerability, contact the repository maintainer privately through GitHub or GitHub's private vulnerability reporting feature if enabled. Do not post secrets or real user data in an issue.

## Deployment caution

The source bundle and automated tests do not certify a live backend deployment as production-secure. Review authentication, authorisation, CORS, rate limiting, provider secrets, database permissions, data retention/deletion and logging before inviting external users.

## AI and user data

Explain when data is sent to a hosted AI provider. Respect the user's explicit consent and configured provider mode. Do not send private browsing histories or identifiers to a provider unless the product has clearly disclosed the processing and the user has consented.
