# NX-421 Mini Project 1 — HCP Language fMRI

Collaborative repository for a five-member EPFL group working in an EPFL VM with Neurodesk.

**Scope:** one subject, one supplied `tfMRI_LANGUAGE_LR` run; Part 1 structural + functional preprocessing and GLM; Part 2 variant 2 spatial ICA.

## Getting started
1. Clone this repository on your EPFL VM.
2. Inspect `dataset_description.md` supplied with the dataset and confirm available Neurodesk tools.
3. Place data in `data/raw/` locally (NEVER commit MRI data).
4. Update `config/paths.example.yaml` or use your own ignored `config/paths.local.yaml`.
5. Run notebooks in numerical order, verifying intermediate outputs before continuing.

## Workflow
1. `01_structural_preprocessing.ipynb` — skull stripping, segmentation, MNI registration.
2. `02_functional_preprocessing.ipynb` — motion/FD, smoothing, alignment QC.
3. `03_glm.ipynb` — design matrix, correlation, task maps and contrasts.
4. `04_ica.ipynb` — ICA spatial maps, first-ten timecourse correlations.

Notebooks are **templates**: no analyses are implemented yet. Record commands, versions, parameter choices and paths before running methods. Avoid hard-coded machine-specific paths.

## Scientific caution
Do not assume supplied fMRI is raw, unregistered, or already MNI aligned. Check its image affine, metadata, visual alignment and dataset documentation. HCP's original language paradigm uses two runs; this assignment lists only the LR run.

## Collaboration
Work on feature branches; open pull requests; ask another member to review. Keep large outputs, NIfTI files, and temporary notebooks out of Git. See `docs/CONTRIBUTING.md`.

## Submission
Course requires a `GROUPNAME_miniproject_1/` folder with `GROUPNAME_report.pdf`, presentation deliverable (confirm recording extension with TA; guideline inconsistently specifies `.pdf`) and `GROUPNAME_code/` containing ordered code files. Verify acceptance of `.ipynb` notebooks or export documented `.py` scripts for final submission. Do not submit data or extra figures.

Deadline: 2026-11-05 at 16:00 Europe/Zurich.
