# Bandelt Dress 2

## A Sum-of-Squares Decomposition for Quartet Covariance

**Full title:** *A Sum-of-Squares Decomposition for Quartet Covariance: Bivariate Independence and Quartet Distance*  
**Authors:** Stefan Grünewald and Libo Huang

This standalone repository contains the PTRF-targeted v8 manuscript and its matched Lean 4 supplementary material. The manuscript snapshot includes the zero-mass-cell copyedit dated 5 September 2026.

本仓库独立保存 PTRF v8 版本的论文、完整 LaTeX 源码和配套 Lean 证明包。论文与证明包保持原版本，不混入旧版 v0.60 材料。

## Read and download

| File | Contents |
|---|---|
| [Grunewald_Huang_PTRF_v8.pdf](Grunewald_Huang_PTRF_v8.pdf) | The 27-page manuscript |
| [Grunewald_Huang_PTRF_v8.tex](Grunewald_Huang_PTRF_v8.tex) | Manuscript LaTeX source |
| [Grunewald_Huang_PTRF_v8_References.bib](Grunewald_Huang_PTRF_v8_References.bib) | Bibliography |
| [Grunewald_Huang_PTRF_v8_Source.zip](Grunewald_Huang_PTRF_v8_Source.zip) | Complete manuscript source package, including class and bibliography-style inputs |
| [ESM_1.zip](ESM_1.zip) | Matched source-only Lean supplement: 142 Lean files, pinned dependencies, correspondence tables, audit records, and licence notices |
| [PTRF_v8_ALIGNMENT_DELIVERY_MANIFEST.txt](PTRF_v8_ALIGNMENT_DELIVERY_MANIFEST.txt) | Preserved version and historical verification record |
| [SHA256SUMS](SHA256SUMS) | Checksums of the six archival files and this README |

## Provenance and version

The six archival files above (excluding this README and `SHA256SUMS`) are byte-for-byte copies of the files previously published in the [original repository's `ptrf-v8` directory](https://github.com/huanglibo389/bandelt-dress-quartet-lean/tree/0b55dc8ee560b4af57bdd43b1f5f09496eacfe57/ptrf-v8). They were copied into this dedicated repository on 11 October 2026. The original repository is retained unchanged; its earlier v0.60 paper and formalization are not included here.

This repository has a new name and its own version history; it does not represent a new revision of the manuscript or the Lean sources. The historical delivery manifest is preserved, including its original date and audit statements.

Before publication, the six archival files were compared with the original public commit, the manuscript hashes in the Lean package's `MANUSCRIPT_LOCK.md` were matched to the manuscript files, and all 156 entries in the supplement's internal `SHA256SUMS` were checked. This transfer does **not** claim a fresh Lean build or a new mathematical review. Historical build and audit records remain inside the supplement.

Publication here does not assert journal acceptance or verify the current status of any journal submission.

## Reproduce the Lean checks

Unpack `ESM_1.zip` and enter `Grunewald_Huang_PTRF_v8_Lean4_Supplement`. Follow its `README.md`, including the pinned Lean/mathlib versions:

```sh
lake exe cache get
lake build
lake env lean BernoulliSupplementAudit.lean
```

See `THEOREM_CORRESPONDENCE.md` for the manuscript-to-Lean map and `MANUSCRIPT_LOCK.md` for the exact manuscript snapshot. Generated `.lake` caches are not included.

To verify the downloaded repository files on macOS:

```sh
shasum -a 256 -c SHA256SUMS
```

## Rights and scope

The manuscript retains its authors' copyright; uploading it here does not apply the Lean code's MIT licence to the paper. The author-written Lean files use the MIT licence included in `ESM_1.zip`, with separate notices for vendored third-party files. The manuscript source package retains the publisher-supplied template's own notices. No new blanket licence is applied by this transfer.

The manuscript's author names, affiliations, and author-contact details are retained as part of the unchanged scholarly manuscript. Submission cover letters, private correspondence, earlier backups, and machine-specific build caches are not included.
