<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Accident-investigation | Contextual (monitoring) | 1.0 | 2/20/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: Argue over all the risks of the autonomous ML system in question.
- **Defeater Description**: If there is an incident with the autonomous ML system, accident investigation should be supported.
- **Source**: Discussion of possible defeaters for an autonomous ML system by a panel of experts.

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: A record of what the autonomous ML system was doing will be necessary in the event of an accident.
- **Underlying Assumptions**: No autonomous ML system can avoid all accidents.
- **Severity / Potential Impact**: Low. Accidents are high impact, but supporting accident investigation by itself is low impact and severity.

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: NA
- **Human (Individual or Team)**: Panel of experts
  - **Expertise / Background**: Experts in automated ML systems and safety.

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: Occurs when accidents occur with the automated ML system.
- **Defeater Frequency**: Only when accidents occur.
- **Phase / Lifecycle Stage**: During testing and operation. 

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: All software systems should allow for logging to aid accident investigation.
- **Operational Context**: All

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Include appropriate and feasible level of logging.
- **Reliability and Validity**: Logging will create information required for accident investigation, but does not guarantee understanding of that accident.
- **Limitations**: Does not prevent accidents, only allows for investigation. Does not help investigation if logging systems do not work.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Logging systems may not work correctly. 

---

## Additional Comments
- **Notes**: Defeater adapted from: R. Bloomfield, G. Fletcher, H. Khlaaf, L. Hinde, and P. Ryan, “Safety Case Templates for Autonomous Systems,” Mar. 11, 2021, arXiv: arXiv:2102.02625. doi: 10.48550/arXiv.2102.02625. 
