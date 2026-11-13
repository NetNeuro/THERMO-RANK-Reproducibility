# THERMO-RANK Reproducibility

Research materials for **Solver-Bound Supervision and Certification Bottlenecks in Coupled Electricity and Heat Dispatch**, by Anfal Hathah and Md. Mottahir Alam.

## Download

Download the named **THERMO_RANK_Reproducibility_v7.zip** asset from [Releases](https://github.com/NetNeuro/THERMO-RANK-Reproducibility/releases). The asset contains the complete runnable research tree, essential datasets, model weights, numerical evidence, figures and editable manuscript sources.

## Scope

The study evaluates solver-bound supervision, first-batch pricing priorities and complete optimization costs under an explicitly specified hypothetical electricity and heat model. It uses public simulated ResStock inputs and an attributed public donor feature dataset. The combined release contains 296 distinct source profiles, 120 added timed dispatch attempts and 1,344 cold pricing attempts, alongside the retained earlier scientific comparisons.

The county and first-batch diagnostics use already frozen models and results. They are exploratory and do not select a favorable county exclusion, model or seed. Improved task selection does not establish uniform end-to-end dispatch acceleration or field-calibrated retrofit savings.

## Reproduce

Extract the release asset and open its THERMO_RANK_Research_v7 folder. Python 3.12 and pinned dependencies are specified in requirements.txt.

```bash
python -m pip install -r requirements.txt
python reproduce.py --verify
python reproduce.py --tests
python reproduce.py --diagnostics /absolute/path/to/NEW_output
python reproduce.py --analyse /absolute/path/to/NEW_full_analysis
python reproduce.py --documents /absolute/path/to/NEW_documents
```

Use a new output directory for each reconstruction. The README inside the asset describes refitting the retained training records and optional fresh timed replays. Recorded primary timings and selected model weights remain unchanged. Pandoc is required only for Word regeneration; rendered PDFs are included.

## Data and rights

ResStock release 2025 Release 1 AMY2018: DOI 10.25984/1876417. Public donor feature dataset: DOI 10.17632/4wgx2mprks.1. Dataset attribution, exact upstream paths, transformations and hashes are included. Third-party datasets retain their original CC BY 4.0 terms.

Read LICENSE_AND_ATTRIBUTION.txt in the release for mixed-source rights and the review/reproduction scope of the authored materials. Third-party manuals and dependency licences retain their own terms; no blanket licence over all mixed-origin files is claimed.

## Verification

SHA256SUMS verifies the packaged research files. Saved schedule constraints, objectives, numerical bound directions, input/model identities and query denominators are checked by the reconstruction scripts. The package retains unsuccessful scientific comparisons and censored outcomes in their proper inventories.
