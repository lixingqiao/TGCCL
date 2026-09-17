# TGCCL

## Tensorized Multi-View Graph Contrastive Learning for Drug Response Prediction

**TGCCL** is a multi-view graph learning framework for anticancer drug response prediction from heterogeneous multi-omics data.

The project investigates how complementary molecular information across multiple omics views can be jointly modeled while incorporating external biological interaction knowledge to improve drug response prediction and generalization.

The corresponding manuscript is currently under revision.

---

## Overview

Drug response prediction aims to estimate the sensitivity of cancer cell lines to anticancer compounds from molecular and drug information.

TGCCL jointly models multiple omics modalities, including:

- gene expression,
- copy-number variation,
- mutation profiles,

together with drug molecular information and biological interaction priors.

The study focuses on representation learning across heterogeneous molecular views and evaluates model robustness under both standard and challenging generalization settings.

---

## Main Results

TGCCL is evaluated on **GDSC2** and independently validated on **CCLE**.

### GDSC2 Warm-Start

Under the warm-start setting, TGCCL achieves:

| Metric | TGCCL |
|---|---:|
| RMSE ↓ | **0.854** |
| MAE ↓ | **0.626** |
| PCC ↑ | **0.954** |

Compared with the strong multi-view graph baseline HMM-GDAN, TGCCL reduces RMSE and MAE by approximately **2.1%** and **2.0%**, respectively.

---

### GDSC2 Cold-Start

TGCCL is further evaluated under more challenging generalization settings in which drugs or cell lines are held out during training.

For the **cold-drug** setting, TGCCL achieves:

| Metric | TGCCL |
|---|---:|
| RMSE ↓ | **2.402** |
| MAE ↓ | **1.835** |
| PCC ↑ | **0.536** |

Compared with HMM-GDAN, RMSE and MAE are reduced by approximately **3.6%** and **5.0%**, respectively.

Additional experiments under the **cold-cell** setting further demonstrate the robustness of TGCCL to unseen biological entities.

---

### Independent Validation on CCLE

On the independent CCLE dataset, TGCCL achieves:

| Metric | TGCCL |
|---|---:|
| RMSE ↓ | **0.879** |
| MAE ↓ | **0.536** |
| PCC ↑ | **0.907** |

The independent-dataset evaluation further demonstrates the cross-dataset robustness of the proposed framework.

---

## Biological Interpretation

In addition to predictive performance, the study investigates the biological relevance of the learned model explanations.

The analysis includes:

- gene-level attribution analysis,
- cross-omics attribution comparison,
- GO enrichment analysis,
- KEGG pathway enrichment analysis.

These analyses are used to examine whether highly attributed genes are associated with biologically relevant pathways and drug-response mechanisms.

---

## Evaluation

The study includes comprehensive evaluation across:

- warm-start prediction;
- cold-drug generalization;
- cold-cell generalization;
- independent-dataset validation;
- ablation studies;
- parameter sensitivity;
- statistical significance analysis;
- biological interpretation;
- computational efficiency analysis.

---

## Research Topics

- Graph Neural Networks
- Multi-View Learning
- Multi-Omics Learning
- Contrastive Learning
- Drug Response Prediction
- Biomedical AI
- Representation Learning

---

## Publication

**Xingqiao Li et al.**

*Tensorized Multi-View Graph Contrastive Learning for Drug Response Prediction*

---

## Code Availability

The core implementation is currently not publicly released because the manuscript is still under peer review and related research materials are being finalized.

The current repository is intended to provide a public overview of the research problem, evaluation protocol, and representative experimental results.

Additional materials may be released after completion of the publication process.

---

## Contact

**Xingqiao Li**  
School of Computer Science, Wuhan University

GitHub: [lixingqiao](https://github.com/lixingqiao)
