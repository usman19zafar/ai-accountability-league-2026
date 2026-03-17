# ALIGN100 Analysis Report

**Document ID:** 711df334  
**Run ID (P7):** fd45704f-ef47-4d07-9ff5-cca1b7327039  
**Generated:** 2026-03-17 09:03 UTC  
**Validation status:** RESEARCH PROTOTYPE  

---

## Accumulated Score Scorecard

### Five-Dimension Composite Score

| Dimension | Score | Weight | Contribution |
|---|---|---|---|
| u(x) Uncertainty | 1.0000 | λ₁ = 0.35 | 0.3500 |
| r(x) Governance Risk | 0.6667 | λ₂ = 0.30 | 0.2000 |
| d(x) Diversity | 1.0000 | λ₃ = 0.20 | 0.2000 |
| v(x) Adversarial | 0.6156 | λ₄ = 0.15 | 0.0923 |
| **a(x) Composite** | **0.8423** | 1.00 | **0.8423** |

### Per-Stage Supporting Metrics

| Stage | Primary | Secondary | Status |
|---|---|---|---|
| P1+P2 Calibration | Brier = 0.2500 | sECE = 0.0000 | Poor |
| P3 Event Extraction | Clusters = 8 | Temporal cov. = 1.000 | OK |
| P4 Relations | SNR = 2.707 | LDR fraction = 0.000 | Good |
| P5 KG Linking | Accept=0 Review=0 Abstain=0 | Mean confidence=0.500 | Low |
| P6 Adversarial | AUC = 0.7500 | Mean p_adv = 0.6156 | Valid |
| P7 Governance | Drift = No | Gold docs = 1 | PROTOTYPE |

---

## 📋 Executive Summary

The document with ID 711df334 is a validated gold document that has undergone pipeline processing. The composite score a(x) is 0.8423, comprising the universality score u of 1.0000, the relevance score r of 0.6667, the diversity score d of 1.0000, and the validity score v of 0.6156. The pipeline stages for acceptance and review have failed, resulting in zero accepted and reviewed documents, which may impact the reliability of downstream results due to the lack of human evaluation, despite the absence of drift and satisfactory calibration and adversarial metrics.

---

## 🔗 Alignment Quality (P1+P2)

The Brier score of 0.2500 and the sECE (static Expected Calibration Error) of 0.0000 provide insights into the model's confidence reliability. A lower Brier score indicates better calibration, with 0 being perfect. However, a score of 0.2500 suggests room for improvement in the model's ability to predict probabilities that reflect real outcomes. The sECE of 0.0000 indicates that the model is well-calibrated, as it measures the difference between the model's predicted probabilities and the true probabilities. This suggests that the model's confidence in its predictions is reliable, but the Brier score indicates that the predictions themselves may not be highly accurate.

---

## 🕸️ Event Graph (P3)

The pipeline context indicates that the event extraction process was successful, with 8 clusters identified. The calibration Brier score is 0.2500, which suggests some degree of miscalibration. However, the adversarial AUC of 0.7500 is a valid measurement, indicating a moderate level of robustness. Additionally, 1 gold document was validated, and no drift was detected. These results provide a foundation for further analysis.

---

## 🔀 Relation Corrections (P4)

The GNN long-distance relation correction results are based on a pipeline context with 8 clusters, which is a satisfactory number. The calibration Brier score is 0.2500, indicating some room for improvement in the model's calibration. However, the adversarial AUC of 0.7500 suggests that the model is performing reasonably well in terms of distinguishing between positive and negative classes. The presence of 1 validated gold document and the absence of drift (drift=no) also contribute to the reliability of the results.

---

## 📚 KG Linking (P5)

Knowledge Graph (KG) linking is a crucial component of our pipeline, enabling the connection of entities and concepts across different data sources. In the current context, we have 8 clusters (OK) and a calibration Brier score of 0.2500, indicating a moderate level of calibration. The adversarial AUC of 0.7500 suggests that our model is reasonably robust against adversarial attacks. However, the accept fraction is 0.000, and the number of accepted, reviewed, and abstained documents are all 0, which raises concerns about the effectiveness of our KG linking process.

---

## 🛡️ Adversarial Safety (P6)

The pipeline context assessment reveals a mixed bag of results. On the positive side, the clusters parameter is set to 8, which is within acceptable limits. The calibration_brier score of 0.2500 has been measured, and the adversarial_auc score of 0.7500 is valid, indicating a reasonable level of performance. Additionally, the gold_docs parameter has been validated with a value of 1, and no drift has been detected. However, it is essential to acknowledge that an auc score of approximately 0.5 would indicate that the detector performed at random chance, and the adversarial dimension v(x) produced no usable signal.

---

## ⚖️ Governance & Final Score (P7)

The final composite score is a(x)=0.8423 and can be broken down into its components: u(x)=1.0000 × λ₁=0.35, r(x)=0.6667 × λ₂=0.30, d(x)=1.0000 × λ₃=0.20, v(x)=0.6156 × λ₄=0.15.

---

