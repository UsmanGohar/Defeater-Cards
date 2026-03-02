# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| BVLOS-DF-02 | Pilot BVLOS Skill | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation)
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – "The operator is capable of safely piloting the BVLOS mission."
* **Defeater Description:** The operator piloting a BVLOS mission must have the necessary experience and training. Insufficient experience could lead to dangerous situations like the sUAS crashing while out of sight.
* **Source:** Poor operator BVLOS ability has been determined to be responsible for accidents reported on flight incident databases like NTSB CAROL.

---

### **Why?** (Justification and Rationale)
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** Threatens the safety of the sUAS and surroundings, including bystanders.
* **Underlying Assumptions:** BVLOS flight is allowed at flight location.
* **Severity/Potential Impact:** Moderate-to-High. Poor operation BVLOS risks harm to the vehicle and surroundings, including bystanders.

---

### **Who?** (Stakeholders, Expertise & Contributors)
*Who are the auditors/reviewers? (e.g., expertise coverage, teams etc.)*

* **Automated:** Flight control software
* **Human:** sUAS manufacturer, operator, regulatory agencies, bystanders.
* **Expertise/Background:** Safety assurance, Piloting experience, BVLOS regulatory compliance.

---

### **When?** (Temporal & Lifecycle Relevance)
*When does the defeater emerge? (e.g., after deployment, etc.)*

* **Event/Trigger:** May occur during flight if pilot is not sufficiently skilled to operate BVLOS.
* **Defeater Frequency:** Has been reported infrequently on government-operated incident report databases (NTSB).
* **Phase:** During operation.

---

### **Where?** (Context and Scope)
*Where within the system or operational context does this defeater apply or manifest?*

* **System/Component:** Operator (?), sUAS hardware, Linked devices.
* **Operational Context:** Pre-flight training/experience.

---

### **How?** (Mitigation & Response)
*How is this defeater detected, monitored, or mitigated?*

* **Monitoring & Mitigation:** Ensure pilot receives sufficient training for BVLOS operation before allowing them to fly.
* **Reliability & Validity:** Analysis of government-operated aviation incident report databases shows instances of BVLOS crashing incidents, including those involving other vehicles, caused by sUAS operator error.
* **Limitations:** Available training time for any given drone model is limited.
* **Residual Risks:** Sensor or communication issues could induce BVLOS issues even for skilled operators. Operators must check these components during the preflight safety check phase.

---