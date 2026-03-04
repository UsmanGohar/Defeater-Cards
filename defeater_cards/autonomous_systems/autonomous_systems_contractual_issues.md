<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Contractual Issues  | Contextual | 1.0 | 2/20/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: Autonomous ML system will be kept up to date in terms of software and hardware.
- **Defeater Description**: Unless there are contractual issues with obtaining software or hardware from a vendor
- **Source**: Discussion of possible defeaters for an autonomous ML system by a panel of experts. 

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: Future contractual issues with obtaining software or hardware are likely, and difficult to predict. Some logic in the safety assurance argument relies on software and hardware being up to date.
- **Underlying Assumptions**: We assume that the system will require software and hardware from outside vendors.
- **Severity / Potential Impact**: This defeater will likely not be a frequent problem, but in certain circumstances could have a severe impact. 

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: NA
- **Human (Individual or Team)**: Panel of experts
  - **Expertise / Background**: Experts in automated ML systems and safety

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: Only when there are contractual issues with obtaining software or hardware.
- **Defeater Frequency**: Infrequent, depending on contract cycles.
- **Phase / Lifecycle Stage**: Operations phase.  

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: All system components that involve updating hardware or software from an outside vendor or through a contract.
- **Operational Context**: Specifically, while updating hardware or software.

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: The company that produces the autonomous ML system must ensure that contracts are kept up to date, and if outside contractors are unable to continue to provide necessary updates and upgrades, find a new contractor.
- **Reliability and Validity**: N/A
- **Limitations**: Ensuring that contracts are in place cannot be guaranteed.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: There is some risk that a contract cannot be in place, or that a contractor will fail in their duties even if one is in place. 

---

## Additional Comments
- **Notes**: Defeater adapted from: R. Bloomfield, G. Fletcher, H. Khlaaf, L. Hinde, and P. Ryan, “Safety Case Templates for Autonomous Systems,” Mar. 11, 2021, arXiv: arXiv:2102.02625. doi: 10.48550/arXiv.2102.02625. 
