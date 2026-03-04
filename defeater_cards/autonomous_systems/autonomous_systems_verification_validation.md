<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Verification and Validation | Evidence Defeater | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: The Adaptive Cruise Control (ACC) has been verified and validated.
- **Defeater Description**: The ACC's verification and validation may not account for all real-world driving scenarios.
- **Source**: Created by GPT-4 based on a series of prompts. Defeaters were then evaluated by three authors who have experience with assurance cases.

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: In complex, real-world environments, not all situations can be accurately simulated during testing
- **Underlying Assumptions**: We assume that the verification and validation techniques are proper and complete.
- **Severity / Potential Impact**: Severe - if the ACC causes an accident this could injure or kill someone.

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: GPT-4, using three levels of prompting about a previously generated assurance case.
- **Human (Individual or Team)**: Filter, repair, and evaluate individual defeaters.
  - **Expertise / Background**: Humans have several years of experience with assurance cases, including in domain-specific topics. GPT-4 received no specific training outside of the prompts used.

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: During verification and validation of the ACC system.
- **Defeater Frequency**: Rare to frequent, depending on the simulations and tests used to verify or validate the ACC system. 
- **Phase / Lifecycle Stage**: V&V.

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: All systems.
- **Operational Context**: V&V

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**:  Increase the set of tests and simulations used for V&V. Perform data gathering research to increase the number of real-world situations that are tested. Include fail safe code for when the ACC encounters unknown situations.
- **Reliability and Validity**: Tests can be performed between the real-world performance of the ACC and the simulated performance to get an idea of the quality of the V&V.
- **Limitations**: No V&V will be complete for all situations.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: All driving involves risks.

---

## Additional Comments
- **Notes**: Defeater adapted from: T. Viger et al., “AI-Supported Eliminative Argumentation: Practical Experience Generating Defeaters to Increase Confidence in Assurance Cases,” in 2024 IEEE 35th International Symposium on Software Reliability Engineering (ISSRE), Oct. 2024, pp. 284–294. doi: 10.1109/ISSRE62328.2024.00035. 
