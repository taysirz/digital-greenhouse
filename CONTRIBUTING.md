# Contributing

## Before changing code

1. Read the root README and the AUREVA product brief.
2. Read the current release notes and engineering documentation in the source archive.
3. Preserve the distinction between implemented behaviour and roadmap items.
4. Keep deterministic protection rules separate from uncertain AI classification.

## Development

- Work from the latest source snapshot in `releases/AUREVA_0.1.4_Developer_Preview.zip`.
- Keep extension and backend tests with their respective components.
- Avoid inline scripts in Manifest V3 extension pages.
- Keep the mini-app to one vertical scroll surface.
- Preserve accessible contrast, keyboard focus and reduced-motion support.

## Testing and claims

Run the relevant package tests and document the result. Manual Chrome verification is separate from automated tests. Do not claim that a feature or release is production-ready unless that status has been verified.

## Secrets

Never commit live API keys, signing secrets, access tokens, private environment files or personal user data.
