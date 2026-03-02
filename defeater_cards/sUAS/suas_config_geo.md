# Defeater Card

### Metadata
| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Config-DF-02 | Geofence Correctness | Contextual | 1.0 | March 2025 | Open |

---

### **What?** (Identification and Evaluation)
*What is being evaluated? (e.g., what argument, evidence, etc.)*

* **Affected Node:** Claim – "All geofences have been correctly set for the given mission."
* **Defeater Description:** Geofences set virtual constraints for sUAS flight area boundaries to prevent flying in unauthorized areas. Incorrect geofence setting could lead to dangerous situations like the sUAS flying unsafely near other air traffic.
* **Source:** Flyaway-related accidents have been reported on flight incident databases like NTSB CAROL. Geofences are a useful tool to help prevent such accidents, but may not be set correctly.

---

### **Why?** (Justification and Rationale)
*Why is this important to the validity or credibility of the argument or evidence?*

* **Rationale:** Flying into unauthorized airspace can be illegal as well as dangerous with a risk of aerial collisions and other accidents.
* **Underlying Assumptions:** Flight control software supports geofences, drone is equipped with GPS sensors.
* **Severity/Potential Impact:** Moderate-to-High. Flying into restricted airspace risks harm to the vehicle and surroundings, including other aerial vehicles.

---

### **Who?** (Stakeholders, Expertise & Contributors)
*Who are the auditors/reviewers? (e.g., expertise coverage, teams etc.)*

* **Automated:** Flight control software
* **Human:** sUAS manufacturer, operator, regulatory agencies, bystanders, other aerial vehicles.
* **Expertise/Background:** Safety assurance, Piloting experience, BVLOS regulatory compliance.

---

### **When?** (Temporal & Lifecycle Relevance)
*When does the defeater emerge? (e.g., after deployment, etc.)*

* **Event/Trigger:** Flight into unauthorized or unsafe areas may occur if operator does not correctly set geofence parameters prior to flight.
* **Defeater Frequency:** Flyaways have been reported on government-operated incident report databases (AAIB) and forum posts. Geofence parameters are commonly used to prevent such behavior, especially in areas near restricted flight zones.
* **Phase:** During operation.

---

### **Where?** (Context and Scope)
*Where within the system or operational context does this defeater apply or manifest?*

* **System/Component:** Flight control software, sUAS hardware, sensors.
* **Operational Context:** Pre-flight parameter tuning, Mission planning.

---

### **How?** (Mitigation & Response)
*How is this defeater detected, monitored, or mitigated?*

* **Monitoring & Mitigation:** Set geofence boundaries and specify geofence actions prior to flight.
* **Reliability & Validity:** Analysis of government-operated aviation incident report databases shows instances of BVLOS crashing incidents, including those involving other vehicles, caused by sUAS operator error.
* **Limitations:** Relies on GPS accuracy.
* **Residual Risks:** Sensor issues or certain PID misconfigurations may still cause geofence violations even if the geofence is set correctly. Operators must check configurations and sensor accuracy prior to flight.

---