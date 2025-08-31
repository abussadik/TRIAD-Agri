# Triad Technologies for Resilient Agribusiness — Open Project

**What**: Public release of datasets, code, figures, and supplementary materials from a 24‑month, 12‑estate deployment of an integrated **AI–IoT–Blockchain** architecture for tropical plantation supply chains.  
**Why**: Enable reuse, reproducibility, and extension of our methods and results.

## Repository Structure
```
triad-agri/
├─ README.md
├─ LICENSE                # Code: MIT; Data: CC BY 4.0
├─ CITATION.cff
├─ CODE_OF_CONDUCT.md
├─ CONTRIBUTING.md
├─ environment.yml  | requirements.txt
├─ .gitignore | .gitattributes (Git LFS for large files)
├─ src/
│  └─ analysis/
│     └─ make_figures.py
├─ notebooks/
│  └─ 01_reproduce_results.ipynb (placeholder)
├─ data/
│  ├─ README.md
│  ├─ processed/      # public CSV/XLSX (non‑sensitive)
│  └─ samples/        # tiny samples/synthetic data
├─ figures/           # exported PNGs
└─ supplementary/     # PPTX, pseudocode, extra tables
```

## Quick Start
```bash
# conda
conda env create -f environment.yml
conda activate triad-agri

# or pip
pip install -r requirements.txt

# Recreate figures
python src/analysis/make_figures.py
```

## Data Dictionary
See `data/README.md` for file details and columns.

## Reproducibility
- Deterministic seeds used in sample generators.
- Figure script relies on CSVs in `data/processed/`.

## Citing
Please cite the repository and the related paper (see `CITATION.cff`).

## Licenses
- **Code**: MIT (see `LICENSE`)
- **Data**: CC BY 4.0 (attribution required)

## Data Availability
All datasets and supplementary materials required to reproduce the public figures are included. Financial and
confidential partner records are excluded; de‑identified summaries or synthetic samples are provided when helpful.
Access to any restricted raw data may be considered under a data‑use agreement.
