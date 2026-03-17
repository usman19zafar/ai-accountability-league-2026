# ALIGN100 Analysis Report

**Document ID:** d83951dc  
**Run ID (P7):** d2f6bff2-830c-4280-bedb-bf3f6ed6373a  
**Generated:** 2026-03-17 07:54 UTC  
**Validation status:** RESEARCH PROTOTYPE  

---

## Accumulated Score Scorecard

### Five-Dimension Composite Score

| Dimension | Score | Weight | Contribution |
|---|---|---|---|
| u(x) Uncertainty | 1.0000 | λ₁ = 0.35 | 0.3500 |
| r(x) Governance Risk | 0.6667 | λ₂ = 0.30 | 0.2000 |
| d(x) Diversity | 1.0000 | λ₃ = 0.20 | 0.2000 |
| v(x) Adversarial | 0.6036 | λ₄ = 0.15 | 0.0905 |
| **a(x) Composite** | **0.8405** | 1.00 | **0.8405** |

### Per-Stage Supporting Metrics

| Stage | Primary | Secondary | Status |
|---|---|---|---|
| P1+P2 Calibration | Brier = 0.2500 | sECE = 0.0000 | Poor |
| P3 Event Extraction | Clusters = 7 | Temporal cov. = 1.000 | OK |
| P4 Relations | SNR = 3.390 | LDR fraction = 0.000 | Good |
| P5 KG Linking | Accept=0 Review=0 Abstain=0 | Mean confidence=0.500 | Low |
| P6 Adversarial | AUC = 0.5000 | Mean p_adv = 0.6036 | RANDOM — no signal |
| P7 Governance | Drift = No | Gold docs = 1 | PROTOTYPE |

### ⚠️ Known Issues This Run

- 🟡 **Adversarial AUC ≈ 0.5**: detector is random; v(x) carries no signal.

---

## 📋 Executive Summary

The document d83951dc is a validated gold document with a composite score of 0.8405, comprising the universality score u=1.0000, the relevance score r=0.6667, the diversity score d=1.0000, and the validity score v=0.6036. The pipeline stages for calibration and adversarial robustness reported a calibration Brier score of 0.2500 and an adversarial AUC of 0.5000, indicating that the adversarial robustness assessment failed to provide meaningful signal. Given the failure in the adversarial robustness stage, the reliability of downstream results, particularly those dependent on the pipeline's ability to withstand adversarial attacks, should be viewed with caution, although the document's validation and other pipeline stages, such as clustering, appear to have performed as expected.

---

## 🔗 Alignment Quality (P1+P2)

The Brier score of 0.2500 and the sECE of 0.0000 provide insight into the model's confidence reliability. A lower Brier score indicates better calibration, with a score of 0 being perfect. However, a score of 0.2500 suggests that the model's predictions may not be entirely reliable. On the other hand, the sECE of 0.0000 indicates that the model is well-calibrated in terms of its expected calibration error, suggesting that the model's confidence is aligned with its accuracy. This discrepancy between the Brier score and sECE highlights the need for further evaluation to understand the model's performance.

---

## 🕸️ Event Graph (P3)

The pipeline context reveals that the event extraction process yielded 7 clusters, indicating a successful extraction of events. The calibration Brier score is 0.2500, which is a measured value. However, the adversarial AUC is 0.5000, suggesting that it is a random result with no signal. The presence of 1 validated gold document provides a baseline for evaluation. With no drift detected, the results can be considered stable.

---

## 🔀 Relation Corrections (P4)

The GNN long-distance relation correction results are based on a pipeline context with 7 clusters, which is a positive indicator. The calibration Brier score of 0.2500 suggests that the model's predictions are reasonably calibrated. However, the adversarial AUC of 0.5000 indicates that the model is not performing better than random, which may be a cause for concern. The presence of 1 validated gold document and the absence of drift are also notable. The signal-to-noise ratio (SNR) of 3.390 and the low LDR fraction of 0.000 suggest that the model is not capturing long-distance relationships effectively.

---

## 📚 KG Linking (P5)

Knowledge Graph (KG) linking is a crucial component of our pipeline, enabling the connection of entities and concepts across different data sources. In our current context, we have a cluster setup with 7 clusters, which is functioning as expected. However, our calibration Brier score is 0.2500, indicating room for improvement in the calibration of our model. The adversarial AUC score of 0.5000 suggests that our model is not effectively distinguishing between legitimate and adversarial examples, which is a significant concern. Despite these challenges, we have validated 1 gold document, which provides a baseline for our evaluation.

---

## 🛡️ Adversarial Safety (P6)

The pipeline context reveals a mixed assessment of performance. On one hand, the clustering process yielded 7 clusters, which is deemed acceptable. Additionally, the calibration Brier score of 0.2500 has been measured, and one gold document has been validated. However, the adversarial AUC of 0.5000 indicates that the detector performed at random chance, suggesting that the adversarial dimension v(x) produced no usable signal. This lack of signal implies that the detector was unable to effectively distinguish between legitimate and adversarial inputs.

---

## ⚖️ Governance & Final Score (P7)

The final composite score is a(x)=0.8405 and can be broken down into its components: u(x)=1.0000 × λ₁=0.35, r(x)=0.6667 × λ₂=0.30, d(x)=1.0000 × λ₃=0.20, v(x)=0.6036 × λ₄=0.15.

---

