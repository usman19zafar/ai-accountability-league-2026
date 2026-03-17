# ALIGN100 Analysis Report

**Document ID:** da7e3c19  
**Run ID (P7):** 34124351-f3d5-47f0-b276-f5ef68a4629e  
**Generated:** 2026-03-17 07:14 UTC  
**Validation status:** RESEARCH PROTOTYPE  

---

## Accumulated Score Scorecard

### Five-Dimension Composite Score

| Dimension | Score | Weight | Contribution |
|---|---|---|---|
| u(x) Uncertainty | 1.0000 | λ₁ = 0.35 | 0.3500 |
| r(x) Governance Risk | 0.6667 | λ₂ = 0.30 | 0.2000 |
| d(x) Diversity | 1.0000 | λ₃ = 0.20 | 0.2000 |
| v(x) Adversarial | 0.6083 | λ₄ = 0.15 | 0.0913 |
| **a(x) Composite** | **0.8413** | 1.00 | **0.8413** |

### Per-Stage Supporting Metrics

| Stage | Primary | Secondary | Status |
|---|---|---|---|
| P1+P2 Calibration | Brier = 0.2500 | sECE = 0.0000 | Poor |
| P3 Event Extraction | Clusters = 8 | Temporal cov. = 1.000 | OK |
| P4 Relations | SNR = 3.646 | LDR fraction = 0.000 | Good |
| P5 KG Linking | Accept=0 Review=0 Abstain=0 | Mean confidence=0.500 | Low |
| P6 Adversarial | AUC = 0.5000 | Mean p_adv = 0.6083 | RANDOM — no signal |
| P7 Governance | Drift = No | Gold docs = 0 | PROTOTYPE |

### ⚠️ Known Issues This Run

- 🟡 **Adversarial AUC ≈ 0.5**: detector is random; v(x) carries no signal.
- 🟡 **No gold documents**: composite score weights are unvalidated defaults.

---

## 📋 Executive Summary

This document is an executive summary of the pipeline context for doc_id da7e3c19. The composite score a(x) is 0.8413, comprising the universality score u of 1.0000, the relevance score r of 0.6667, the diversity score d of 1.0000, and the veracity score v of 0.6083. The pipeline stages for calibration and adversarial robustness failed, with a high calibration_brier score of 0.2500 and a random adversarial_auc of 0.5000, which may impact the reliability of downstream results, including the composite score, due to uncalibrated weights and lack of signal.

---

## 🔗 Alignment Quality (P1+P2)

The Brier score of 0.2500 and the sECE of 0.0000 provide insight into the confidence reliability of the model. The Brier score measures the mean squared error between predicted probabilities and actual outcomes, with lower values indicating better calibration. However, a Brier score of 0.2500 suggests that there is room for improvement in terms of the model's ability to produce reliable confidence estimates. On the other hand, the sECE of 0.0000 indicates that the model is well-calibrated in terms of its expected calibration error, which is a measure of the difference between the model's predicted probabilities and its actual accuracy.

---

## 🕸️ Event Graph (P3)

The pipeline context indicates that the event extraction process was successful, with 8 clusters identified. The calibration Brier score is 0.2500, which suggests some level of calibration in the model. However, the adversarial AUC is 0.5000, indicating no signal and random performance. Additionally, there are 0 gold documents, which means the weights are uncalibrated. The absence of drift is a positive sign, but the lack of coreference with a score of 0.000 is a limitation.

---

## 🔀 Relation Corrections (P4)

The GNN long-distance relation correction results are based on a pipeline context with 8 clusters, which is a positive indicator. However, the calibration Brier score of 0.2500 suggests that there is room for improvement in terms of calibration. The adversarial AUC of 0.5000 indicates no signal, which may be a cause for concern. Additionally, the absence of gold documents and the presence of uncalibrated weights may impact the accuracy of the results.

---

## 📚 KG Linking (P5)

Knowledge Graph (KG) linking is a crucial component of our pipeline, enabling the connection of entities in unstructured text to a comprehensive knowledge base. However, our current pipeline context reveals some challenges in this area. With accept_frac=0 and n_abstained=0, it appears that our KG linking process is not currently accepting any links, but this is not due to abstentions. The absence of a loaded KG index or failures in P3 event extraction could both potentially lead to such an outcome, but in this case, we must consider the specifics of our pipeline context to understand the root cause.

---

## 🛡️ Adversarial Safety (P6)

The pipeline context reveals a mixed assessment of the system's performance. With 8 clusters, the system is functioning as expected in terms of data organization. However, the calibration_brier score of 0.2500 indicates room for improvement in terms of calibration. Furthermore, the adversarial_auc score of 0.5000 suggests that the detector performed at random chance, and the adversarial dimension v(x) produced no usable signal. This lack of signal does not necessarily imply a lack of threat, but rather that the system was unable to effectively detect or respond to potential threats.

---

## ⚖️ Governance & Final Score (P7)

The final composite score is a(x)=0.8413 and can be broken down into its components: u(x)=1.0000 × λ₁=0.35, r(x)=0.6667 × λ₂=0.30, d(x)=1.0000 × λ₃=0.20, v(x)=0.6083 × λ₄=0.15.

---

