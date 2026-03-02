# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Battery-DF-01 | Battery Charge | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation) 
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – *"The state of charge of the battery is sufficient for safe flight."*
* **Defeater Description:** A sufficiently charged battery is required for safe operation. An operator may fail to check the charge level of the battery prior to flight. This can lead to flight failure if the remaining charge is insufficient for the required mission.
* **Source:** Battery failure reports are widespread on government flight incident databases. Failure of operator to properly check the battery state is frequently cited as a cause of such incidents.

---

### **Why?** (Justification and Rationale) 
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** Threatens the capability of the sUAS to complete its planned mission.
* **Underlying Assumptions:** sUAS is battery operated.
* **Severity/Potential Impact:** Moderate-to-High. Battery failure during flight can cause damage to the vehicle and may pose a risk to bystanders in the vicinity.

---

### **Who?** (Stakeholders, Expertise & Contributors) 
*Who are the auditors/reviewers? (e.g., expertise coverage, teams etc.)*

* **Automated:** Flight control software
* **Human:** sUAS manufacturer, operator, regulatory agencies, bystanders.
* **Expertise/Background:** Safety assurance, Piloting experience, Aviation regulatory compliance.

---

### **When?** (Temporal & Lifecycle Relevance) 
*When does the defeater emerge? (e.g., after deployment, etc.)*

* **Event/Trigger:** May emerge during flight if adequate battery charge is not checked by operator prior to flight or experiences unexpected failure.
* **Defeater Frequency:** Appears frequently on government-operated incident report databases (like NTSB CAROL or AAIB).
* **Phase:** During operation.

---

### **Where?** (Context and Scope) 
*Where within the system or operational context does this defeater apply or manifest?*

* **System/Component:** sUAS hardware, Battery.
* **Operational Context:** Pre-flight safety check.

---

### **How?** (Mitigation & Response) 
*How is this defeater detected, monitored, or mitigated?*

* **Monitoring & Mitigation:** Manually check battery charge level in the field before each takeoff. Do not take off unless battery allows for sufficient flight time to perform planned mission.
* **Reliability & Validity:** Analysis of government-operated aviation incident report databases reveals that up to 15% of reported incidents may be caused by battery issues, including failure by the operator to correctly check the charge level prior to flight.
* **Limitations:** Battery health degrades over time.
* **Residual Risks:** Unexpected battery failures are possible even with correct preflight safety checks. Operators must ensure that batteries are replaced with sufficient frequency.

---