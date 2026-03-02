# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Payload-DF-02 | Payload Secure | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation)
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – "The sUAS is capable of safely carrying the given payload weight for the duration of the mission."
* **Defeater Description:** If the sUAS is carrying a payload, it must be attached securely. A payload may be attached incorrectly or unsecurely. This may cause it to fall during flight.
* **Source:** Payload-related failures have been reported on government flight incident databases.

---

### **Why?** (Justification and Rationale)
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** Threatens the success of the mission and the safety of the surroundings, including bystanders.
* **Underlying Assumptions:** Flying with payload attached is allowed at flight location.
* **Severity/Potential Impact:** Moderate-to-High. Payload may fall, posing a risk to bystanders in the vicinity.

---

### **Who?** (Stakeholders, Expertise & Contributors)
*Who are the auditors/reviewers? (e.g., expertise coverage, teams etc.)*

* **Automated:** Flight control software
* **Human:** sUAS manufacturer, operator, regulatory agencies, bystanders.
* **Expertise/Background:** Safety assurance, Piloting experience, Aviation regulatory compliance.

---

### **When?** (Temporal & Lifecycle Relevance)
*When does the defeater emerge? (e.g., after deployment, etc.)*

* **Event/Trigger:** May emerge at any time during flight.
* **Defeater Frequency:** Has been reported infrequently on government-operated incident report databases (AAIB).
* **Phase:** During operation.

---

### **Where?** (Context and Scope)
*Where within the system or operational context does this defeater apply or manifest?*

* **System/Component:** sUAS hardware, Payload.
* **Operational Context:** Pre-flight safety check.

---

### **How?** (Mitigation & Response)
*How is this defeater detected, monitored, or mitigated?*

* **Monitoring & Mitigation:** Verify that payload is securely attached during pre-flight safety check.
* **Reliability & Validity:** Analysis of government-operated aviation incident report databases reveals that just over 1% of reported accidents may be caused by payload-related issues.
* **Limitations:** Reliant on sUAS hardware integrity.
* **Residual Risks:** Hardware failure related to attachment system may still occur. Operator should check hardware components for signs of stress or breakage regularly. Payload must not be over the maximum weight capacity of the sUAS.

---