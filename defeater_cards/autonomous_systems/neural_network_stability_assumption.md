<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Stability Assumption | Uncertainty | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: In the context of a Neural Network Detection Computer (NN-Detect-Comp) (for extracting the part of a video or still image that is an airport runway). Believing: Verification is correct and complete to the Foreseeable Operating Conditions (FOC) {IT-Testdata}, To these premises: 1. Stability is shown through data never seen in the training but belongs to trained scenarios
- **Defeater Description**: Stability assumption does not hold
- **Source**: Experts at Daedalean (a Swiss AI in aerospace company) working with the FAA and EASA

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: If the Neural Net (NN) does not behave in a stable manner when exposed to training data it never saw, then the NN-Detect-Comp will likely be unable to operate in the uncertainty of the real world.
- **Underlying Assumptions**: The data never seen in training is similar to the rest of the training data, and is similar to the FOC and Operational Design Domain (ODD)
- **Severity / Potential Impact**: Potentially harmful, if the instability of the neural network leads to incorrect location of the runway during landing. 

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

- **Event / Trigger**: Validation during training. 
- **Defeater Frequency**: Uncommon
- **Phase / Lifecycle Stage**: Training

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: NN-Detect-Comp
- **Operational Context**: NN training and validation

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Ensure all neural networks are validated on data in the training set that was randomly withheld from training, to ensure stability. 
- **Reliability and Validity**: Given sufficient training data, this verification can be very reliable. 
- **Limitations**: Verification is limited to the breadth of the training data. 
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Low

---

## Additional Comments
- **Notes**: Defeater adapted from: T. Varchev, S. Staudacher, Z. Daw, and M. Holloway, “Arguing machine learning assurance for certification,” Software Engineering 2025–Companion Proceedings, 2025, doi: 10.18420/SE2025-WS-09.
