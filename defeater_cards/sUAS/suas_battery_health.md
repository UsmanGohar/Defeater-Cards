# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Battery-DF-02 | Battery Health | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation)
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – "The state of charge and health of the battery is sufficient for safe flight."
* **Defeater Description:** A healthy battery is required for safe operation. A battery may lose its capacity for charge or inflate due to age or damage. Inflated or otherwise damaged batteries are not safe for use, and unexpectedly fast drain due to low capacity can also cause failure during flight.
* **Source:** Battery failure reports are widespread on government flight incident databases, including battery health related issues such as abnormal drain.

---

### **Why?** (Justification and Rationale)
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** Threatens the capability of the sUAS to fly safely.
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

* **Event/Trigger:** May emerge during flight if battery experiences unexpected failure due to age or damage.
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

* **Monitoring & Mitigation:** Manually check battery health before flying. Check for signs of bloating or damage before each takeoff. Keep replacement batteries available.
* **Reliability & Validity:** Analysis of government-operated aviation incident report databases reveals that up to 15% of reported incidents may be caused by battery issues, including those related to abnormal drain, a sign of poor health due to age.
* **Limitations:** Battery health degrades over time.
* **Residual Risks:** Unexpected battery failures are possible even with correct preflight safety checks. Operators must ensure that batteries are replaced with sufficient frequency.

---