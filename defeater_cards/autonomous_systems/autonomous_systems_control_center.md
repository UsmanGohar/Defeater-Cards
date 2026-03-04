<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [Defeater ID] | Communication with control center  | Contextual | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: There is evidence of the resilience of the AI (of the unmanned diving marine vessel) in knowing how the control of the vessel is and it is always communicated with the control center.
- **Defeater Description**: Communications problems with the control center might exist
- **Source**: Discussion of possible defeaters from a panel of marine experts. 

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: The assurance argument assumes that the vessel is always communicating with the control center. That may not be possible in all situations. 
- **Underlying Assumptions**: Communications are not always reliable.
- **Severity / Potential Impact**: Potentially severe

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Panel of experts.
  - **Expertise / Background**: Experts in marine systems and AI.

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: Communication disruption with the control center when the AI marine vessel requires it
- **Defeater Frequency**: Depending on communication protocol, communication lapses could be relatively common or rare. 
- **Phase / Lifecycle Stage**: Deployment/testing

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: AI control program
- **Operational Context**: During operation

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Create multiple redundant communication pathways. Ensure the unmanned diving vessel has a safe fail-state in the event of a long-term loss of communication. 
- **Reliability and Validity**: Multiple redundant communication systems are effective during 99% of test operations.
- **Limitations**: Extreme or unusual environmental conditions both increase the likelihood of communication failure and the consequences of that failure. 
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Communication loss still possible on any platform.

---

## Additional Comments
- **Notes**: Defeater adapted from : L.-P. Cobos, T. Miao, K. Sowka, G. Madzudzo, A. R. Ruddle, and E. El Amam, “Application of an Automotive Assurance Case Approach to Autonomous Marine Vessel Security,” in 2022 International Conference on Electrical, Computer, Communications and Mechatronics Engineering (ICECCME), Maldives, Maldives: IEEE, Nov. 2022, pp. 1–9. doi: 10.1109/ICECCME55909.2022.9988376. 
