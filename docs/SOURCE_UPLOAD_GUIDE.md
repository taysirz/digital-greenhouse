# Add the complete AUREVA 0.1.4 source tree

The complete source-import kit is prepared as a separate ZIP in this conversation. It contains the extension and backend files, release artifacts, per-file hashes and a PowerShell helper that clones the correct branch, merges the source folders, checks for secrets, and commits/pushes after an explicit confirmation.

## Prepared source-import kit

- File: `TOLEVU_AUREVA_GitHub_Source_Import_0.1.4.zip`
- SHA-256: `f5a13bf37b72ba25200273351fa3b14038b38a72ed3e67b2cd985bc02ba37835`
- Contains 92 extension files, 34 backend files, 2 versioned release ZIPs, release notes and `SOURCE_SHA256_MANIFEST.txt`.
- Includes `PUSH_TO_GITHUB.ps1` for the final upload on Windows.

## One-step Windows upload

1. Download and extract the source-import kit.
2. Install Git for Windows if it is not already installed.
3. Open PowerShell in the extracted folder.
4. Run:

   ```powershell
   powershell -ExecutionPolicy Bypass -File .\PUSH_TO_GITHUB.ps1
   ```

5. The helper clones or updates `taysirz/digital-greenhouse`, checks out `aureva-0.1.4`, merges the source directories without overwriting this branch's existing documentation, checks for common secret/runtime files, stages the code, shows a summary and asks you to type `PUSH` before committing and pushing.

GitHub authentication uses your local Git Credential Manager / Git setup. No GitHub token is embedded in the script.

## Target

Repository: https://github.com/taysirz/digital-greenhouse  
Branch: `aureva-0.1.4`  
Draft PR: https://github.com/taysirz/digital-greenhouse/pull/1

## What is included

- `AUREVA/extension/` — Manifest V3 extension source, HTML, CSS, JavaScript, JSON, icons, rules and tests.
- `AUREVA/backend/` — Node.js backend, dashboards, storage, scripts and tests.
- `AUREVA/release-notes/` — current brand system, start guide and test report.
- `releases/` — exact AUREVA 0.1.4 Chrome-ready and Developer Preview ZIPs.
- `SOURCE_SHA256_MANIFEST.txt` — integrity hashes for every source file.

## Security and release boundary

- Do not merge the draft PR into `main` until the source has been reviewed and public release is intended.
- The kit contains no `.env` files, provider credentials, production database or user browsing records. The helper performs a further check before staging.
- `extension/service-config.js` contains the previously configured hosted service origin for compatibility. It is not a credential; verify it is still an intended endpoint before distribution.
- Automated tests passed according to the included 0.1.4 report; manual Chrome acceptance remains pending.
- The 0.1.4 patch does not change the scoring engine. The eight-hour/zero-points issue remains open.
