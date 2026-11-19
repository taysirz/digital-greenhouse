# AUREVA releases

## 0.1.4 — Plant-first visual and CSP/scroll patch

**Status:** Prepared local release artifacts; GitHub binary uploads remain outstanding.

### Artifacts

| Artifact | Local size | SHA-256 |
|---|---:|---|
| Chrome Ready | 342,849 bytes | `21b506995cf27e1556000a6e240ca6745b06a55137643f2b2e22aa9d5de55c6e` |
| Developer Preview | 450,758 bytes | `535cf3d4c82546730edbcfaa68b2908cd74652f2b1e2b2807eb05e98df2116fe` |

The Developer Preview contains the extension source, backend source, tests and documentation. The Chrome Ready package contains the installable extension.

### Changes

- Popup dashboard-mode bootstrap moved out of inline script into local `view-mode.js` to comply with Manifest V3 CSP.
- Full-tab mini-app changed to a single document-level vertical scroll surface.
- Final colour hierarchy layer added in `extension/aureva-polish.css`.
- Existing colour tokens and product logic retained.

### Test boundary

The included test report states that automated checks passed. It specifically calls for manual Chrome acceptance of:
1. Popup CSP error no longer appearing.
2. A single visible vertical scrollbar in the full-tab mini-app.
3. Sticky navigation while scrolling.
4. Colour placement across the plant, weather, digital-life, care, Focus, Protect, Coach and Setup surfaces.

The scoring engine, points rules, Focus, protection, privacy, sync and backend behaviour were not changed in this patch. The user's reported eight-hour/zero-points experience is still an open issue.

### Important

The binary ZIP packages are not currently stored in this GitHub branch. Their hashes are recorded here so a later upload can be checked against the prepared artifacts.
