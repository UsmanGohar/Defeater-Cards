<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | Navigation Problems | Contextual | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: AI of an unmanned diving marine vessel is operationally safe
- **Defeater Description**: Unless there are problems with the navigation system.
- **Source**: Discussion of possible defeaters from a panel of marine experts.

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: The navigation system of an unmanned diving marine vessel is vital to the safe operation of that vessel. If the vessel cannot navigate, then it may collide with other vessels, obstacles, etc. or become lost and unable to return to a safe state where humans can intervene.
- **Underlying Assumptions**: The navigation system is the only system on board that can help the underwater vessel to safely move around. 
- **Severity / Potential Impact**: Major

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Panel of experts
  - **Expertise / Background**: Major

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: When navigation system fails.
- **Defeater Frequency**: Given sufficient redundancy, a complete loss of navigation system should be extremely rare.
- **Phase / Lifecycle Stage**: Operations/testing

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: Navigation system (all)
- **Operational Context**: During operation

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Ensure navigation system has redundancy and self-diagnoses and repair. Try to ensure the vehicle is fail-safe in case of navigation failure.
- **Reliability and Validity**: Navigation subsystem failure should be made to be extremely rare (10-9 per usage hour or less) through redundancy and self-diagnosis.
- **Limitations**: Difficult to protect from total system failure based on common cause failure types. Ensuring all vehicles are up to date with their software and hardware can be difficult with a large fleet.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**:Navigation system failure still possible. It can be difficult to ensure a navigation system is fail-safe.

---

## Additional Comments
- **Notes**: Defeater adapted from: L.-P. Cobos, T. Miao, K. Sowka, G. Madzudzo, A. R. Ruddle, and E. El Amam, “Application of an Automotive Assurance Case Approach to Autonomous Marine Vessel Security,” in 2022 International Conference on Electrical, Computer, Communications and Mechatronics Engineering (ICECCME), Maldives, Maldives: IEEE, Nov. 2022, pp. 1–9. doi: 10.1109/ICECCME55909.2022.9988376.
