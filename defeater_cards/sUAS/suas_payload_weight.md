# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Payload-DF-01 | Payload Weight | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation)
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – "The sUAS is capable of safely carrying the given payload weight for the duration of the mission."
* **Defeater Description:** If the sUAS is carrying a payload, the weight should be within safe limits. An excessively heavy payload may be attached in error. Flight failure may occur if the payload is too heavy.
* **Source:** Payload-related failures have been reported on government flight incident databases.

---

### **Why?** (Justification and Rationale)
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** Threatens the safety of the sUAS and surroundings.
* **Underlying Assumptions:** Flying with payload attached is allowed at flight location.
* **Severity/Potential Impact:** Moderate-to-High. Payload may fall or cause a crash, damaging the vehicle and posing a risk to bystanders in the vicinity.

---

### **Who?** (Stakeholders, Expertise & Contributors)
*Who are the auditors/reviewers? (e.g., expertise coverage, teams etc.)*

* **Automated:** Flight control software
* **Human:** sUAS manufacturer, operator, regulatory agencies, bystanders.
* **Expertise/Background:** Safety assurance, Piloting experience, Aviation regulatory compliance.

---

### **When?** (Temporal & Lifecycle Relevance)
*When does the defeater emerge? (e.g., after deployment, etc.)*

* **Event/Trigger:** May emerge at takeoff time if payload is too heavy to fly; else may manifest during flight if payload falls or causes crash.
* **Defeater Frequency:** Has been reported infrequently on government-operated incident report databases (AAIB).
* **Phase:** During operation.

---

### **Where?** (Context and Scope)
*Where within the system or operational context does this defeater apply or manifest?*

* **System/Component:** sUAS hardware, Payload.
* **Operational Context:** Mission planning, Pre-flight safety check.

---

### **How?** (Mitigation & Response)
*How is this defeater detected, monitored, or mitigated?*

* **Monitoring & Mitigation:** Specify maximum payload capacity during mission planning. Verify payload is under limit during safety check.
* **Reliability & Validity:** Analysis of government-operated aviation incident report databases reveals that just over 1% of reported accidents may be caused by payload-related issues.
* **Limitations:** Dependent on accurate reporting of sUAS weight bearing capacity.
* **Residual Risks:** Payload must be securely attached to avoid falling during flight. Operators must ensure that payload is secure during safety check.

---