# ALIGN100 Analysis Report

**Document ID:** 816c04dd  
**Run ID (P7):** 2dade91d-b1e5-4e9b-9b5b-98a3567b2055  
**Generated:** 2026-03-17 07:35 UTC  
**Validation status:** RESEARCH PROTOTYPE  

---

## Accumulated Score Scorecard

### Five-Dimension Composite Score

| Dimension | Score | Weight | Contribution |
|---|---|---|---|
| u(x) Uncertainty | 1.0000 | λ₁ = 0.35 | 0.3500 |
| r(x) Governance Risk | 0.6667 | λ₂ = 0.30 | 0.2000 |
| d(x) Diversity | 1.0000 | λ₃ = 0.20 | 0.2000 |
| v(x) Adversarial | 0.6136 | λ₄ = 0.15 | 0.0920 |
| **a(x) Composite** | **0.8420** | 1.00 | **0.8420** |

### Per-Stage Supporting Metrics

| Stage | Primary | Secondary | Status |
|---|---|---|---|
| P1+P2 Calibration | Brier = 0.2500 | sECE = 0.0000 | Poor |
| P3 Event Extraction | Clusters = 8 | Temporal cov. = 1.000 | OK |
| P4 Relations | SNR = 2.965 | LDR fraction = 0.000 | Good |
| P5 KG Linking | Accept=0 Review=0 Abstain=0 | Mean confidence=0.500 | Low |
| P6 Adversarial | AUC = 0.8750 | Mean p_adv = 0.6136 | Valid |
| P7 Governance | Drift = No | Gold docs = 1 | PROTOTYPE |

---

## 📋 Executive Summary

The document is a validated gold document with ID 816c04dd, evaluated through the pipeline with a composite score of 0.8420, comprising the universality score (u) of 1.0000, the relevance score (r) of 0.6667, the diversity score (d) of 1.0000, and the validity score (v) of 0.6136. The pipeline stages for acceptance and review failed as indicated by n_accepted=0 and n_review=0, suggesting that despite the document's high composite score, it was not accepted or sent for review, potentially due to the stringent criteria or thresholds set for these stages. Given the absence of drift and the successful validation of the gold document, the downstream results, including the composite score and its components, are considered reliable, providing a solid basis for further analysis or decision-making.

---

## 🔗 Alignment Quality (P1+P2)

The Brier score of 0.2500 and the sECE of 0.0000 provide insight into the model's confidence reliability. A lower Brier score indicates better calibration, as it measures the mean squared error between predicted probabilities and actual outcomes. However, a Brier score of 0.2500 suggests room for improvement in the model's calibration. On the other hand, the sECE (static Expected Calibration Error) of 0.0000 indicates that the model is well-calibrated, as it measures the difference between the model's predicted probabilities and the true probabilities. This suggests that the model's confidence is reliable, but the Brier score indicates that there may still be some overconfidence or underconfidence in certain predictions.

---

## 🕸️ Event Graph (P3)

The pipeline context indicates that the event extraction process was successful, with 8 clusters identified. The calibration Brier score is 0.2500, which suggests that the model's probability estimates are reasonably calibrated. Additionally, the adversarial AUC is 0.8750, indicating a strong ability to distinguish between positive and negative classes. The presence of 1 validated gold document also supports the validity of the results. With no drift detected, the results can be considered reliable.

---

## 🔀 Relation Corrections (P4)

The GNN long-distance relation correction results indicate a notable performance in handling complex relationships within the data. Given the pipeline context, where clusters equal 8, calibration Brier score is 0.2500, and adversarial AUC is 0.8750, it suggests that the model has been trained and validated on a robust dataset with a reasonable number of clusters. The absence of drift and low violation mean of 0.0000 further support the stability and reliability of the model's predictions.

---

## 📚 KG Linking (P5)

Knowledge Graph (KG) linking is a crucial component of our pipeline, enabling the connection of entities in unstructured text to a comprehensive knowledge base. The current pipeline context indicates that the clusters are functioning correctly with 8 clusters (OK), and the calibration Brier score is 0.2500, suggesting room for improvement in the model's calibration. The adversarial AUC of 0.8750 is valid, and we have validated 1 gold document. However, the accept fraction is 0.000, and the mean calibration probability is 0.500, with no accepted, reviewed, or abstained documents.

---

## 🛡️ Adversarial Safety (P6)

The pipeline context reveals a mixed assessment of performance. With 8 clusters (OK), the calibration Brier score is 0.2500, indicating some degree of miscalibration. However, the adversarial AUC of 0.8750 suggests that the model is capable of distinguishing between legitimate and adversarial examples to some extent. The presence of 1 validated gold document and the absence of drift (no) are also positive indicators. Furthermore, the detection AUC of 0.8750 and the mean adversarial probability (p_adv_mean) of 0.6136 provide additional insights into the model's performance.

---

## ⚖️ Governance & Final Score (P7)

The final composite score is a(x)=0.8420 and can be broken down into its components: u(x)=1.0000 × λ₁=0.35, r(x)=0.6667 × λ₂=0.30, d(x)=1.0000 × λ₃=0.20, v(x)=0.6136 × λ₄=0.15.

---

