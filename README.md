# Math Exports Release Audit

This repository holds the export batch prepared for the Atlas 2025-11 public data release.

- `exports/eval_mathmix_1k.jsonl` — curated evaluation-style math instruction sample.
- `exports/vendor_mathgen_500.jsonl` — vendor-format math generation sample.

Both exports were produced by the ingestion tooling from public NVIDIA math instruction
corpora. The tooling records only the source batch fingerprint at ingest time; the mapping
from a fingerprint to the upstream collection is maintained in the governance archive
snapshot shipped with this repository:

- `registry/atlas_governance_archive_cd331d42.html`
- published mirror: https://raw.githubusercontent.com/knobbyintens/huggingface_github_terminal_fetch_yahoo-finance_playwright_with_chunk_8050-audit-d4fa77/main/registry/atlas_governance_archive_cd331d42.html

Neither export carries a licence column and this README intentionally does not state one.
Per-file batch metadata is recorded in `docs/export_manifest.json`.
