<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Inaccurate Control Model Tests | Uncertainty | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: S4 Control model test results (of the Construction Zone Assist (CZA) module of the Automatic Driving System (ADS)).
- **Defeater Description**: UM7 Unless the results were recorded inaccurately
- **Source**: Panel of safety experts

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: The test results of the control module are not useful if they are recorded inaccurately.
- **Underlying Assumptions**: The control module tests are capable of being recorded inaccurately. 
- **Severity / Potential Impact**: Potentially extremely severe, but unlikely.

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

- **Event / Trigger**: Testing
- **Defeater Frequency**: Frequency depends on how well the control module tests are designed and recorded.
- **Phase / Lifecycle Stage**: Testing

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: Control Module
- **Operational Context**: Testing

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Verify control module tests are correctly recording results.
- **Reliability and Validity**: High-quality control module tests should ensure results are almost always recorded correctly.
- **Limitations**: N/A
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: N/A

---

## Additional Comments
- **Notes**:
