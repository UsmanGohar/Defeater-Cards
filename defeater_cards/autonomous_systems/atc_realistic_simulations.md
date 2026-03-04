<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Realistic Simulations | Evidence Validity | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: E0017 Software simulation results showing that ATC software detects 99% of duplicate SSR codes within D seconds. (&) S0028 Argue over reasons that the simulation might be invalid 
- **Defeater Description**: D0022 But the simulations might not have considered a realistic breadth of operating (challenge) circumstances
- **Source**: Panel of experts in aviation management

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: If the simulations do not have a realistic breadth of operating circumstances, then the simulation does not greatly add to our assurance that the system will work in realistic situations.
- **Underlying Assumptions**: Assumes that the software simulation is a reasonable proxy for actual software functioning. 
- **Severity / Potential Impact**: Potentially harmful. Could cause confusion of ATC or pilots in the airspace, which might create dangerous situations.

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Experts from Raytheon Canada.
  - **Expertise / Background**: Experts in air traffic control and software systems.

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: During testing, if sufficiently realistic simulations have not been created.
- **Defeater Frequency**: Rare
- **Phase / Lifecycle Stage**: Testing

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: ATC Software, SSR code assignment module.
- **Operational Context**: Testing

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Analyze simulation scripts for realistic hazards, derive simulation scripts from real-world ATC situations. 
- **Reliability and Validity**: Highly reliable.
- **Limitations**: Cannot account for all situations. 
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Low. Although not all risks can be eliminated, we have high confidence the simulations will cover almost all real-world situations. 

---

## Additional Comments
- **Notes**: Defeater adapted from: S. Diemert, J. Goodenough, J. Joyce, and C. Weinstock, “Incremental Assurance Through Eliminative Argumentation,” Journal of System Safety, vol. 58, no. 1, pp. 7–15, Mar. 2023, doi: 10.56094/jss.v58i1.215.
