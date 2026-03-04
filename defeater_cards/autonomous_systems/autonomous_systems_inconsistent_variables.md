<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Inconsistent Variables | Uncertainty | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: G7 Longitudinal and lateral control variables are well-defined in the Construction Zone Assist (CZA) module of the Automatic Driving System (ADS). 
- **Defeater Description**: R7.1 Unless the variables are inconsistent or inadequately tested in certain operational conditions
- **Source**: Panel of safety experts.

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: If the variables are not tested correctly, then the existence of the variables does not increase the safety of the system.
- **Underlying Assumptions**: Operational conditions will affect variable performance.
- **Severity / Potential Impact**: Potentially extremely severe, if inconsistent variables cause accidents while in construction zones.

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Panel of experts
  - **Expertise / Background**: Automotive Safety

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: Automatic driving in a construction zone in operational conditions that have not been correctly tested.
- **Defeater Frequency**: Rare - only in very specific unforeseen circumstances.
- **Phase / Lifecycle Stage**: During deployment or testing. 

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: Longitudinal and lateral control. 
- **Operational Context**: Specific unforeseen circumstances.

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Increase testing of these variables. Create other operational conditions for these variables.
- **Reliability and Validity**: Include testing of new variable testing to assess reliability. 
- **Limitations**: Cannot ensure complete reliability of these variables.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Not all operational conditions can be foreseen.

---

## Additional Comments
- **Notes**: Defeater adapted from: N. Laxman, J. Jiby, I. Sorokos, J. Frey, and J. Reich, From Uncertainty Representation to Safety Performance Monitoring for Operational Safety Assurance -A Systematic Approach. 2025. doi: 10.3850/978-981-94-3281-3_ESREL-SRA-E2025-P8451-cd
