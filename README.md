# Ultimate Ticker Tape — v4.4.0 known-good freeze

Bill selected SpaceArt UltimateTicker v4.4.0 (BillRing Edition) as the smoothest build. This branch preserves the exact recovered HTML, with no animation, styling, feed, or behavior edits.

## Open the frozen build

Download `index.html` and open it in a browser. It is byte-identical to [the named frozen original](frozen/v4.4.0/SpaceArt_UltimateTicker_v4.4.0.html). For GitHub downloads, use the raw/download-file action rather than saving the GitHub page.

## Version reconciliation

| Version | Evidence and disposition |
| --- | --- |
| v3.0–v3.2 | Recovered classic builds, preserved under `archive/classic/`. |
| v3.3 | Original main commit `c1bc661c2defb1050392c33a49331920ce3e8ad5`, dated September 4, 2026. Its `index (3).html` exactly matches the recovered named v3.3 build by Git blob SHA. That original root file remains intact. |
| v3.4 | Recovered named build matches the Library copy by SHA-256. Drive also lists this filename and size. |
| v3.5 / v3.5.1 | Classic DuckWalk and Hardening Edition builds recovered and preserved. Drive lists both, so v3.4 is not the newest classic file there. |
| v4.0.0–v4.3.0 | SpaceArt development snapshots, preserved under `archive/spaceart/`. |
| v4.4.0 | Selected known-good baseline. Two prior workspace copies and the Library copy have identical SHA-256. Its About text identifies the v3.5.1 feed foundation. |
| v4.4.1 OrbitStudy / v4.5.0 / v4.6.0 | Preserved under `archive/experiments/`; their higher version numbers do not replace Bill's v4.4.0 choice. |

The repository's main branch had only the initial README and v3.3 upload commits when inspected. The later recovered builds were absent from main. The classic ticker and SpaceArt ring presentation are distinct development stages; this import does not invent intermediate Git history or claim all historical features are equivalent.

## Integrity and preservation

- Dedicated branch: `freeze/v4.4.0-known-good`; main remains unchanged.
- Parent: the existing v3.3 commit. All original history remains reachable.
- 16 distinct named HTML builds are preserved, plus the two root aliases.
- [FREEZE_MANIFEST.json](FREEZE_MANIFEST.json) records provenance, sizes, SHA-256 and Git blob identities.
- [SHA256SUMS](SHA256SUMS) covers every preserved HTML file. Run `sha256sum -c SHA256SUMS` from the repository root to verify a download.
- Frozen v4.4.0 SHA-256: `5c975a1678ef4083639c54e0c043039fbb149d3877ac33495ea6a8fb14b76a0f`.

This is a byte-preservation freeze, not a new release of the animation. Live news, third-party endpoints, fonts and browser-local preferences can still change. Bill's smoothness assessment is the selection evidence; this freeze does not claim fresh performance measurements. Inline JavaScript syntax and artifact identities were checked during preparation.

Keep this branch as a reference snapshot. Start future edits on a separate branch from its freeze commit; use the commit permalink as the permanent reference because branch names can move. No production deployment or main-branch merge is included in this freeze.
