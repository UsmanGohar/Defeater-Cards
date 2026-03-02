# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Config-DF-01 | Correct PID Tuning | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation)
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – "The flight parameter configuration being used produces stable flight behavior"
* **Defeater Description:** A correctly tuned PID controller maintains stability during flight. An operator may fail to check or enter incorrect PID controller values. Incorrect PID parameter configurations can cause unsafe behavior like instability, deviation, and crashing.
* **Source:** PID misconfigurations have been reported in forum posts and NTSB incident reports. Impact of incorrect PID tuning has been studied in simulated and real-world environments, detected with real-time instability monitoring as well as post-flight log file analysis.

---

### **Why?** (Justification and Rationale)
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** The argument presumes that pre-flight parameter tuning improves flight behavior. However, when tuning is performed incorrectly, dangerous behavior can occur.
* **Underlying Assumptions:** Flight control software allows tuning by the operator.
* **Severity/Potential Impact:** Moderate-to-High. Failures such as instability and crashing have been shown to cause damage to the vehicle and may pose a risk to bystanders in the vicinity.

---

### **Who?** (Stakeholders, Expertise & Contributors)
*Who are the auditors/reviewers? (e.g., expertise coverage, teams etc.)*

* **Automated:** Flight control software, Simulator
* **Human:** sUAS manufacturer, operator, flight control software developer, regulatory agencies, bystanders.
* **Expertise/Background:** Safety assurance, Piloting experience, Aviation regulatory compliance.

---

### **When?** (Temporal & Lifecycle Relevance)
*When does the defeater emerge? (e.g., after deployment, etc.)*

* **Event/Trigger:** Occurs during flight when pre-flight tuning is not performed correctly.
* **Defeater Frequency:** Appears intermittently in posts on flight control software forums and infrequently on government-operated incident report databases (like NTSB CAROL).
* **Phase:** During operation.

---

### **Where?** (Context and Scope)
*Where within the system or operational context does this defeater apply or manifest?*

* **System/Component:** Flight control software, PID controller, sUAS hardware.
* **Operational Context:** Pre-flight PID tuning.

---

### **How?** (Mitigation & Response)
*How is this defeater detected, monitored, or mitigated?*

* **Monitoring & Mitigation:** Validate configurations with simulation prior to real-world flight. Manually check configuration in the field before flying. Monitor flight state to ensure PID controller is functioning correctly and adapt by reconfiguring if instability is detected.
* **Reliability & Validity:** Reconfiguration-based adaptation approaches have been shown to recover from misconfigurations in simulation and real-world case studies.
* **Limitations:** Knowledge base of configuration behavior is limited.
* **Residual Risks:** Residual risk remains and must be handled by more drastic adaptation strategies such as landing in place if crashing is likely.

---