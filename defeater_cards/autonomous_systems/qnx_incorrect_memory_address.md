<!-- Adapted from the Huggingface Model Card template: https://github.com/huggingface/huggingface_hub/blob/main/src/huggingface_hub/templates/modelcard_template.md -->

# Defeater Card

## Metadata: ##

Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | SM Incorrect Memory Address | Contextual | 1.0 | 2/22/26 | Open |

---

## What? *(Identification and Evaluation)*  
**What is being evaluated?**  
(e.g., what argument, evidence, or reasoning step is affected?)

- **Affected Claim / Evidence Node**: C0067 When the Startup Verifier (SV) transfers control of the System on a Chip (SoC) to the Blackberry QNX Operating System (QOS) it will transfer control to the correct start instruction.
- **Defeater Description**: D0142 Unless the Startup Module (SM) incorrectly patched the SV's boot data structure such that it points to an incorrect address in memory
- **Source**: Blackberry engineers and experts in operating systems.

---

## Why? *(Justification and Rationale)*  
**Why is this important to the validity or credibility of the argument or evidence?**

- **Rationale**: Starting the boot process at the wrong location in memory could mean that the startup process starts with incorrect or malicious code.
- **Underlying Assumptions**: The SM contains the location in memory to begin the boot structure, and this location can be changed. 
- **Severity / Potential Impact**: Starting at the incorrect memory location is an extremely severe security risk. 

---

## Who? *(Stakeholders, Expertise & Contributors)*  
**Who are the auditors or reviewers?**  
(e.g., expertise coverage, teams, roles)

- **Automated**: N/A
- **Human (Individual or Team)**: Experts at Blackberry
  - **Expertise / Background**: Expertise in security and operating systems

---

## When? *(Temporal & Lifecycle Relevance)*  
**When does the defeater emerge?**  
(e.g., after deployment, under stress conditions)

- **Event / Trigger**: When the SM is complete and is handing control of the system over to the SV. 
- **Defeater Frequency**: Rare
- **Phase / Lifecycle Stage**: Testing and operation

---

## Where? *(Context and Scope)*  
**Where within the system or operational context does this defeater apply or manifest?**

- **System / Component**: The Startup Module and Startup Verifier
- **Operational Context**: During system boot

---

## How? *(Mitigation & Response)*  
**How is this defeater detected, monitored, or mitigated?**

- **Monitoring & Mitigation**: Have the SV verify the integrity of its own executable code prior to running any other checks. If this check fails, abort the system boot.
- **Reliability and Validity**: Extremely high, depending on the method of integrity checking of the SV.
- **Limitations**: This is only as secure as the method of integrity checking used.
  <!--(e.g., sociotechnical factors, disagreements, project constraints)-->
- **Residual Risks**: Very low.

---

## Additional Comments
- **Notes**: Defeater derived from: C. Hobbs, S. Diemert, and J. Joyce, “Driving the Development Process from the Safety Case,” Safety Critical Systems Club, 2024. 
