<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Erroneous Element | Uncertainty | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: C0012 The Startup Verifier (SV) will safely transfer control of the System on a Chip (SoC) to the Blackberry QNX Operating System (QOS). 
- **Defeater Description**: D0024 Unless the SV detects an erroneous element and incorrectly transfers control of the SoC to the QOS when it should enter a terminal state.
- **Source**: Blackberry engineers and experts in operating systems

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: The security of the SoC relies on the correct operation and hand-off between the SV and QOS. If this does not work correctly, then the startup process may have been compromised, leading to serious security concerns.
- **Underlying Assumptions**: We assume that the SV is capable of detecting erroneous elements during startup.
- **Severity / Potential Impact**: Potentially harmful. The security of the SoC could be compromised if the SV to QOS handoff does not work correctly. 

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Experts at Blackberry.
  - **Expertise / Background**: Expertise in security and operating systems. 

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: During startup
- **Defeater Frequency**: Rare
- **Phase / Lifecycle Stage**: Testing and operation

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: Startup Verifier
- **Operational Context**:

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Ensure when the SV detects an erroneous element, it will enter a terminal state, and will not transfer control to the QOS. 
- **Reliability and Validity**: High reliability.
- **Limitations**: This only works on erroneous elements that the SV can detect. However, the SV can likely detect almost all erroneous elements.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Minimal

---

## Additional Comments
- **Notes**: Defeater derived from: C. Hobbs, S. Diemert, and J. Joyce, “Driving the Development Process from the Safety Case,” Safety Critical Systems Club, 2024. 
