<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Data Not Representative | Evidence Validity | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: In the context of a Neural Network Detection Computer (NN-Detect-Comp) (for extracting the part of a video or still image that is an airport runway) Believing: The training and validation data is representative with regard to Operational Design Domain (ODD) {IT-Data}. To this premise: Augmented data is statistically representative and address possible computer vision challenging situations.: 1. Data and augmented data set distribution are representative to the ODD.
- **Defeater Description**: Unless the Data is not representative of the ODD.
- **Source**: Experts at Daedalean (a Swiss AI in aerospace company) working with the FAA and EASA

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: If the training data for a neural network is not representative of the Operational Design Domain, then the resulting neural network will not function will not function correctly on real-world inputs.
- **Underlying Assumptions**: We assume that having representative data in the training set will result in a functioning neural net.
- **Severity / Potential Impact**: Potentially severe, if the NN Detect Comp cannot correctly identify runways in images in situations when we are relying on it to do so. 

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

- **Event / Trigger**: When training the NN, as well as when using the NN. 
- **Defeater Frequency**: Only if the data is not representative. 
- **Phase / Lifecycle Stage**: Training and flight. 

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: NN Detect Comp
- **Operational Context**: Neural network training

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Prior to training, ensure that the data used for training covers a complete and representative sample of the ODD. (ODD requirements are spelled out in the safety argument.)
- **Reliability and Validity**: Moderately reliable. No review of training data can ensure perfect coverage, but a training data can be improved by careful selection and review.
- **Limitations**: No NN or training data can be ideal, there will always be gaps.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: The ODD might change in the future, and better technologies might make the training data set not representative of what the cameras on the airplanes will be seeing. 

---

## Additional Comments
- **Notes**: Defeater adapted from: T. Varchev, S. Staudacher, Z. Daw, and M. Holloway, “Arguing machine learning assurance for certification,” Software Engineering 2025–Companion Proceedings, 2025, doi: 10.18420/SE2025-WS-09. 
