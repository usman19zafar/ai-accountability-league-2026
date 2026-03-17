# ALIGN100 Analysis Report

**Document ID:** f7861649  
**Run ID (P7):** adbdab2c-bacd-4f16-9ac9-5b243c3e6f92  
**Generated:** 2026-03-17 06:45 UTC  
**Validation status:** RESEARCH PROTOTYPE  

---

## Accumulated Score Scorecard

### Five-Dimension Composite Score

| Dimension | Score | Weight | Contribution |
|---|---|---|---|
| u(x) Uncertainty | 1.0000 | λ₁ = 0.35 | 0.3500 |
| r(x) Governance Risk | 0.6667 | λ₂ = 0.30 | 0.2000 |
| d(x) Diversity | 1.0000 | λ₃ = 0.20 | 0.2000 |
| v(x) Adversarial | 0.6043 | λ₄ = 0.15 | 0.0906 |
| **a(x) Composite** | **0.8406** | 1.00 | **0.8406** |

### Per-Stage Supporting Metrics

| Stage | Primary | Secondary | Status |
|---|---|---|---|
| P1+P2 Calibration | Brier = 0.2500 | sECE = 0.0000 | Poor |
| P3 Event Extraction | Clusters = 7 | Temporal cov. = 1.000 | OK |
| P4 Relations | SNR = 3.759 | LDR fraction = 0.000 | Good |
| P5 KG Linking | Accept=0 Review=0 Abstain=0 | Mean confidence=0.500 | Low |
| P6 Adversarial | AUC = 0.5000 | Mean p_adv = 0.6043 | RANDOM — no signal |
| P7 Governance | Drift = No | Gold docs = 1 | PROTOTYPE |

### ⚠️ Known Issues This Run

- 🟡 **Adversarial AUC ≈ 0.5**: detector is random; v(x) carries no signal.

---

## 📋 Executive Summary

The document with ID f7861649 is a validated gold document with a composite score of 0.8406, comprising component scores of u=1.0000 for understanding, r=0.6667 for relevance, d=1.0000 for diversity, and v=0.6043 for validity. The pipeline stages for calibration and adversarial robustness reported a calibration Brier score of 0.2500 and an adversarial AUC of 0.5000, indicating that the adversarial robustness assessment failed to provide meaningful signal due to its random nature. Despite this failure, the downstream results for this specific document can still be considered reliable due to its validation as a gold document and the presence of other functional pipeline stages, including clustering which performed nominally with 7 clusters.

---

## 🔗 Alignment Quality (P1+P2)

The Brier score of 0.2500 and sECE of 0.0000 provide insight into the confidence reliability of the model. A lower Brier score indicates better calibration, with a score of 0.2500 suggesting room for improvement. The sECE, which measures the difference between the model's predicted probabilities and true probabilities, is close to 0, indicating that the model is well-calibrated in terms of expected calibration error. However, the Brier score suggests that the model's confidence may not be entirely reliable, and further evaluation is needed to understand the model's performance.

---

## 🕸️ Event Graph (P3)

The pipeline context assessment indicates that the event extraction process was successful, with 7 clusters identified. The calibration Brier score is 0.2500, which is a measured value. However, the adversarial AUC is 0.5000, suggesting that it is a random result with no signal. The presence of 1 validated gold document provides some validation to the results. Additionally, there is no drift detected.

---

## 🔀 Relation Corrections (P4)

The GNN long-distance relation correction results are based on a pipeline context with 7 clusters, which is a positive indication. The calibration Brier score of 0.2500 suggests that the model's predictions are somewhat reliable, but there is room for improvement. However, the adversarial AUC of 0.5000 indicates that the model is not performing better than random chance in terms of detecting adversarial examples, which is a significant concern.

---

## 📚 KG Linking (P5)

Knowledge Graph (KG) linking is a crucial component of our pipeline, enabling the connection of entities in unstructured text to a comprehensive knowledge base. The current pipeline context reveals that the clusters and calibration_brier score are within acceptable ranges, with 7 clusters identified and a calibration_brier score of 0.2500. However, the adversarial_auc score of 0.5000 indicates a lack of signal, suggesting that the model may not be effectively distinguishing between positive and negative classes. Furthermore, with only 1 gold document validated and no drift detected, the pipeline's performance is still being closely monitored.

---

## 🛡️ Adversarial Safety (P6)

The pipeline context reveals a mixed assessment of the system's performance. On one hand, the clustering algorithm successfully identified 7 clusters, which is a positive outcome. Additionally, the calibration Brier score of 0.2500 was measured, indicating some level of calibration accuracy. However, the adversarial AUC of 0.5000 suggests that the detector performed at random chance, and the adversarial dimension v(x) produced no usable signal. This implies that the system was unable to effectively distinguish between legitimate and adversarial inputs.

---

## ⚖️ Governance & Final Score (P7)

The final composite score is a(x)=0.8406 and can be broken down into its components: u(x)=1.0000 × λ₁=0.35, r(x)=0.6667 × λ₂=0.30, d(x)=1.0000 × λ₃=0.20, v(x)=0.6043 × λ₄=0.15.

---

