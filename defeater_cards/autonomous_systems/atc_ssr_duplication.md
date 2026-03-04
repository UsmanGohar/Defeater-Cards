<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | SSR Duplication | Requirements | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: S0002 Argue over reasons that non-unique SSR codes might appear in the [air traffic control (ATC)] system
- **Defeater Description**: D0003 Unless an aircraft with an in-use SSR enters the airspace and its code is not reassigned in X seconds
- **Source**: Panel of experts in aviation management

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: The SSR codes for ATC are supposed to be unique. The system in question is supposed to identify non-unique SSR codes quickly. There might be reasons why the system is unable to do so.
- **Underlying Assumptions**: SSR codes should be unique. The system is checking for SSR code uniqueness.
- **Severity / Potential Impact**: Potentially harmful. Could cause confusion of ATC or pilots in the airspace, which might create dangerous situations.

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Experts from Raytheon Canada
  - **Expertise / Background**: Experts in air traffic control and software systems.

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: When an aircraft enters some airspace with a duplicate SSR code. 
- **Defeater Frequency**: Uncommon
- **Phase / Lifecycle Stage**: In use by ATC

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: ATC software system that assigns SSR codes
- **Operational Context**: During flights into ATC-controlled airspace.

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Software testing, simulation, field data, for both detecting duplicates and assigning new SSR codes.
- **Reliability and Validity**: High reliability.
- **Limitations**: The software system must be running and functioning correctly.  
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Minimal

---

## Additional Comments
- **Notes**: Defeater adapted from: S. Diemert, J. Goodenough, J. Joyce, and C. Weinstock, “Incremental Assurance Through Eliminative Argumentation,” Journal of System Safety, vol. 58, no. 1, pp. 7–15, Mar. 2023, doi: 10.56094/jss.v58i1.215. 
