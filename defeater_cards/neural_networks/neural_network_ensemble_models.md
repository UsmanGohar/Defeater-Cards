<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Ensemble Models | Uncertainty | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: In the context of a Neural Network Detection Computer (NN-Detect-Comp) (for extracting the part of a video or still image that is an airport runway). Believing: NN-Detect-Comp holds the component holds Innocuity {Innocuity}. To these premises: Aleatory uncertainty is mitigated through 4 ensemble models {IO-Ensemble}
- **Defeater Description**: Ensemble not working as intended
- **Source**: Experts at Daedalean (a Swiss AI in aerospace company) working with the FAA and EASA

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: An ensemble of neural networks can handle real-world randomness better than a single model, However, if the ensemble is not trained correctly, or is composed of overly similar models, then its effectiveness can be greatly reduced. 
- **Underlying Assumptions**: The ensemble will be more effective than a single model.
- **Severity / Potential Impact**: Potentially somewhat harmful, if some randomness affects the model's detection abilities. 

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Experts at Daedalean in coordination with experts at the FAA and EASA
  - **Expertise / Background**: Experts in machine learning and aviation safety and regulation.

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: During use, when the models are queried to get multiple calculations of runway location. 
- **Defeater Frequency**: Rare. Only when some aleatory effects affect multiple models at once. 
- **Phase / Lifecycle Stage**: In operation.

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: NN models
- **Operational Context**:

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Perform multiple tests on the models to ensure they can handle aleatory uncertainty. Ensure training is separate and not overly correlated.
- **Reliability and Validity**:
- **Limitations**: Given the randomness being addressed by the initial argument, it is difficult to ensure complete
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Minimal. 

---

## Additional Comments
- **Notes**: Defeater adapted from: T. Varchev, S. Staudacher, Z. Daw, and M. Holloway, “Arguing machine learning assurance for certification,” Software Engineering 2025–Companion Proceedings, 2025, doi: 10.18420/SE2025-WS-09. 
