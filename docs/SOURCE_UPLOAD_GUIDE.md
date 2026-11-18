# Add the complete AUREVA 0.1.4 source tree

The GitHub connector used to create this documentation branch cannot transfer local binary archives or recursively add local directories. The prepared source import package is therefore supplied separately for the maintainer to push.

## Package contents

- `AUREVA/extension/` — 92 files: Manifest V3 extension source, interfaces, styles, icons, rules and tests.
- `AUREVA/backend/` — 34 files: Node.js backend, storage, dashboards, scripts and tests.
- `AUREVA/release-notes/` — start-here, automated test and brand notes.
- `releases/` — exact 0.1.4 Developer Preview and Chrome Ready ZIP archives.
- `SOURCE_SHA256_MANIFEST.txt` — hashes for the unpacked AUREVA source files.
- `UPLOAD_TO_GITHUB.md` — maintainer upload steps.

## Target branch

`aureva-0.1.4` in [taysirz/digital-greenhouse](https://github.com/taysirz/digital-greenhouse/tree/aureva-0.1.4).

## Important

Merge the package's AUREVA folder with the existing AUREVA documentation folder. Do not overwrite the existing Markdown documents. Review all files before pushing because the repository is public. Keep real secrets, user data, local databases and production environment files out of Git.
