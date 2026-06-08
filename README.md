# Semantic-Comparison-of-Architectural-Terms-A-Computational-Contextual-Analysis

Public repository for the materials, code, statistical outputs, logs, figures, and runtime records associated with:

**Semantic Comparison of Architectural Terms: A Computational Contextual Analysis**

This study applies a contextual BERT-based semantic comparison framework to selected architectural, conceptual, and aesthetic term pairs. It tests whether paired terms behave as equivalents, oppositions, overlapping concepts, asymmetric semantic fields, or near-fused terms under paired **FULL** and **CLEAN** corpus conditions.

The comparison battery includes six term pairs:

```text
engawa / veranda
tsuboniwa / impluvium
shōji / fusuma
tokonoma / chigaidana
ma / mu
wabi / sabi
```

The repository is intended as a reproducibility and supplementary-materials record for the reported run, not as a general-purpose software package.

## Repository Description

This repository preserves the implementation record and generated materials for a computational contextual analysis of architectural terms. It includes the main analysis script, YAML settings, runtime log, package list, master CSV outputs, master PDF outputs, generated plots, manuscript plots, and edited figures used in the paper.

The study uses pre-declared concept fields and paired FULL/CLEAN corpus audits to examine semantic overlap, dominance, divergence, and near-fusion across architectural and conceptual term pairs.

## Repository Contents

The repository contains the following main files and archives:

```text
LICENSE
Library list.txt
Master CSVs and Master PDFs...
Paper 3 Script.txt
Paper 3 Yaml Settings.txt
Plots Used in the paper.rar
README.md
paper3.log
```

## Main Files

### `Paper 3 Script.txt`

Main analysis script for the reported Paper 3 run.

The script performs the contextual semantic comparison workflow, including:

```text
target-pair processing
concept-field comparison
FULL/CLEAN corpus audit
contextual BERT embedding extraction
bootstrap comparison
permutation testing
multiple-testing correction
master CSV export
figure generation
runtime logging
```

For rerunning, this file can be renamed as:

```text
paper3_pipeline.py
```

### `Paper 3 Yaml Settings.txt`

Main YAML settings file for the reported run.

This file contains the configuration used by the script, including target pairs, concept-field settings, model paths, corpus paths, runtime options, bootstrap settings, plotting settings, and output controls.

For rerunning, this file can be renamed as:

```text
config.yaml
```

### `Library list.txt`

Python package list from the environment used when the script was run.

This file records the installed libraries and their versions at runtime. It is included so that readers can inspect the computational environment used for the reported results.

### `paper3.log`

Runtime log from the reported execution of the script.

The log records the script run sequence, loaded settings, corpus and model access, processing stages, statistical calculations, generated outputs, warnings, and final export steps.

### `Master CSVs and Master PDFs...`

Archive or folder containing the consolidated statistical outputs from the reported run.

These materials contain the main statistical information for the study, including master result tables, comparison outputs, support classifications, confidence intervals, p-values, adjusted values, and manuscript-facing result summaries.

The master CSV files should be treated as the numerical source of record for the reported analysis.

### Master plots

The master plots contain the generated plots from the script, including plots produced during statistical calculation and diagnostic output generation.

These plots preserve the direct computational output before manuscript editing.

### `Plots Used in the paper.rar`

Archive containing the plots used in the paper.

This archive includes both:

```text
original generated plots
modified or edited manuscript plots
```

The original generated plots are preserved for reproducibility. The modified plots are the versions prepared for manuscript presentation.

### `LICENSE`

Repository license file.

This repository uses a dual-license structure:

```text
MIT License for software code
CC BY 4.0 for author-created non-code research materials
```

Third-party materials, source texts, pretrained models, external datasets, and libraries remain governed by their own licenses and terms.

## Study Overview

The study examines whether selected architectural, conceptual, and aesthetic term pairs can be evaluated through controlled semantic evidence rather than interpretive analogy alone.

The analysis compares six term pairs across pre-declared concept fields. Each pair is tested under two corpus conditions:

| Corpus condition | Description                                                                            |
| ---------------- | -------------------------------------------------------------------------------------- |
| `FULL`           | Original corpus condition preserving the broader explanatory corpus.                   |
| `CLEAN`          | Corpus condition after removal of glossary-like and explicitly definitional sentences. |

The FULL/CLEAN audit tests whether semantic patterns remain visible after direct definitional scaffolding is reduced.

## Analytical Workflow

The reported workflow follows five main stages.

### 1. Inherited Analytical Base

The study uses the inherited FULL/CLEAN corpus framework and fine-tuned BERT model from the earlier reproducibility framework.

The model is not retrained for this study. It is used as the contextual representation source for all pairwise comparisons.

### 2. Target Pair Selection

The study tests six predefined pairs:

```text
engawa / veranda
tsuboniwa / impluvium
shōji / fusuma
tokonoma / chigaidana
ma / mu
wabi / sabi
```

The pairs are grouped into three analytical families:

```text
cross-cultural architectural comparisons
within-culture architectural comparisons
conceptual and aesthetic comparisons
```

### 3. Pair-Specific Concept Fields

Each pair is tested against pre-declared concept fields.

Examples include:

```text
indoor-outdoor boundary
perimeter circulation
miniature garden
rainwater catchment
opaque partition
formal shoin setting
temporal pause
nothingness and nonbeing
impermanence and melancholy
```

The concept fields are operational probes. They are not treated as complete dictionary definitions.

### 4. Contextual BERT Comparison

The analysis extracts contextual representations from target-term and concept-field contexts.

For each concept field, the script compares the two paired terms against the same concept centroid.

The directional comparison identifies which term is more strongly associated with the tested concept field.

### 5. Bootstrap, Permutation, and Support Classification

The script estimates directional stability through bootstrap resampling and statistical testing.

The reported results classify support using tiers such as:

```text
strong
suggestive
no clear split
low support
```

The outputs are then exported as master CSV files, master plots, manuscript-facing figures, and logs.

## Main Results Summary

The reported study finds that the tested pairs do not behave as simple equivalents or simple oppositions.

Broadly:

```text
engawa / veranda
```

shows partial overlap, but engawa is more strongly tied to interior-exterior mediation, while veranda is more strongly tied to circulation and sheltered outdoor use.

```text
tsuboniwa / impluvium
```

shows limited equivalence. Tsuboniwa leans toward miniature garden meanings, while impluvium is more strongly associated with water, basin, and Roman domestic-system fields.

```text
shōji / fusuma
```

shows a fusuma-dominant pattern across the tested partition vocabulary.

```text
tokonoma / chigaidana
```

remains mostly weak or non-separating, except for formal shoin setting, which favors chigaidana.

```text
ma / mu
```

shows a clear bidirectional conceptual split between interval-oriented and nothingness-oriented fields.

```text
wabi / sabi
```

remains tightly coupled across most fields, with separation mainly around impermanence and melancholy.

## Generated Outputs

The repository preserves several output types:

```text
master statistical CSV files
master PDF outputs
generated plots
statistical diagnostic plots
original manuscript plots
edited manuscript plots
runtime logs
library/version records
YAML configuration settings
analysis script
```

The master CSV files contain the main statistical information for the reported run and should be used when checking numerical results.

The plot archives preserve both direct script-generated visualizations and the edited versions used in the paper.

## How to Inspect the Results

To inspect the reported run without rerunning the script:

1. Download or clone the repository.
2. Open `paper3.log` to inspect the runtime sequence.
3. Open `Library list.txt` to check the package environment.
4. Inspect the master CSV files for statistical results.
5. Inspect the master PDF files and master plots for generated visual outputs.
6. Open `Plots Used in the paper.rar` to compare original generated plots with the edited manuscript figures.
7. Use `Paper 3 Yaml Settings.txt` to verify the active configuration used for the run.

## How to Rerun the Pipeline

To rerun the pipeline, rename the uploaded files as follows:

```text
Paper 3 Script.txt         ->  paper3_pipeline.py
Paper 3 Yaml Settings.txt  ->  config.yaml
```

Then run:

```bash
python paper3_pipeline.py
```

The exact corpus paths, model paths, output folders, and runtime switches are defined in the YAML settings file.

## Python Environment

The file `Library list.txt` records the Python package environment used for the reported run.

Key libraries used by the study include:

```text
torch
transformers
tokenizers
numpy
pandas
scipy
scikit-learn
spaCy
regex
PyYAML
matplotlib
tqdm
Pillow
safetensors
accelerate
```

Exact versions should be taken from `Library list.txt`.

## Reproducibility Notes

The repository is designed to preserve the reported computational run.

The following files are especially important for reproducibility:

```text
Paper 3 Script.txt
Paper 3 Yaml Settings.txt
Library list.txt
paper3.log
Master CSVs and Master PDFs...
Master plots
Plots Used in the paper.rar
```

Exact numerical replication may depend on local hardware, CUDA version, PyTorch version, Transformers version, model checkpoint files, and corpus availability.

The master CSV files should be treated as the primary numerical record. The plots are visual summaries derived from those outputs.

## Suggested Citation

Please cite the associated paper and repository when using these materials:

```text
Gjata G. and Yamada S. (2026). Semantic Comparison of Architectural Terms: A Computational Contextual Analysis. GitHub repository: https://github.com/ArchiScrub/Semantic-Comparison-of-Architectural-Terms-A-Computational-Contextual-Analysis
```

## License

This repository uses a dual-license structure.

Software code written by the authors is licensed under the MIT License, unless explicitly stated otherwise.

Author-created non-code research materials are licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0), unless explicitly stated otherwise.

Author-created non-code materials include configuration files, documentation, generated summary tables, generated metrics, logs, manifests, original figures, edited manuscript figures, and other research outputs created for this study.

This license does not apply to third-party materials, external source texts, pretrained models, datasets, software libraries, or quoted or extracted text from copyrighted sources. Those materials remain governed by their own licenses, terms, or copyright status.

Where CSV files contain representative contexts, excerpts, or sentence-level material derived from source texts, those textual excerpts are included only for scholarly transparency and reproducibility. They are not relicensed by this repository unless explicitly stated.

The license in this repository does not override the licenses or terms of any third-party materials used in or referenced by the study.

## Third-Party Libraries

The scripts in this repository depend on external Python libraries, including but not limited to:

```text
torch
transformers
tokenizers
numpy
pandas
scipy
scikit-learn
spaCy
regex
PyYAML
matplotlib
tqdm
Pillow
safetensors
accelerate
```

Those libraries are not covered by the licenses in this repository. They retain their own upstream licenses.

## Repository Status

This repository preserves the materials for the reported run of **Semantic Comparison of Architectural Terms: A Computational Contextual Analysis**.

It is intended as a reproducibility and supplementary-materials repository, not as a maintained software package.
