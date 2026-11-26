# Runbook: Digest and Where to Publish

This board uses the shared STEMEd+ pipeline. For how every board works and the common fixes, see the [stemedplus-theme runbook](https://github.com/stemedplus/stemedplus-theme/blob/main/RUNBOOK.md).

| | |
|---|---|
| **Site** | stemedplus.github.io/STEMEd-Digest (and `/publish.html`) |
| **Repository** | stemedplus/stemed-digest |
| **Updates** | Daily at 10:23 UTC, on push, and by hand (`update.yml`) |
| **Sources** | Crossref, by ISSN, for 96 journals in `config/journals.json`; EdArXiv and arXiv in `config/preprints.json`; OpenAlex for dissertations; KC Works for the STEMEd+ Library |
| **Keywords** | `config/keywords.json` decides what counts as STEM+ education |
| **Secret** | `OPENALEX_API_KEY` in the repository's Actions secrets (recommended, free from OpenAlex) |
| **Add or fix** | **Suggest a journal** issue form; add to `config/journals.json` and `config/venues.json` |

**OpenAlex errors:** check the key hasn't expired. Rotate it if anyone with access leaves (see the Access Inventory).

**A journal's articles stopped appearing:** check its ISSN in `config/journals.json` against Crossref; publishers sometimes change ISSNs.

_Written November 2026. Review with the yearly December review._
