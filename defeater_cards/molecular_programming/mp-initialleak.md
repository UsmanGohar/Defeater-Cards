# Defeater Card

## Metadata

| Defeater ID | Defeater Tag | Defeater Type | Version | Date | Status |
|------------|--------------|---------------|--------|------|--------|
| LC-08 | Substoichiometric Leak | Uncertainty | 1.0 | Aug 2025 | Open |

---

## What? (Identification and Evaluation)
*What is being evaluated?*

* **Affected Node:** G1.3 "The substoichiometric yield due to initial leak is at an accepted level."
* **Defeater Description:** The goal assumes that substoichiometric yield loss due to initial leak is bounded within an acceptable level. However, imperfections such as truncated strands, synthesis errors, and incomplete annealing can produce defective gate complexes that are spuriously reactive and participate in unintended strand-displacement reactions immediately at system initialization.
* **Source:** Initial fluorescence spikes and early input consumption observed during experimental initialization of DNA strand-displacement circuits \cite{Lapteva22}.

---

## Why? (Justification and Rationale)
*Why is this important to the validity of the argument?*

* **Rationale:** Initial leak causes premature consumption of input strands at $t \approx 0$, distorting the stoichiometric relationship between input and output species. This leads to systematic underestimation of effective input concentration and biases yield measurements, undermining claims about correctness and quantitative behavior of the CRN.
* **Underlying Assumptions:** Assumes that a non-negligible population of defective species (e.g., truncated or misfolded strands) persists after preparation and can participate in unintended reactions.
* **Severity/Potential Impact:** Moderate. Can lead to premature depletion of reactants and degraded circuit fidelity, particularly in cascaded or multi-stage systems. Experimental studies of DNA strand-displacement systems report initial leak fractions on the order of $10^{-2}$ to $10^{-1}$.

---

## Who? (Stakeholders, Expertise & Contributors)

* **Automated:** Fluorescence time-series analysis and kinetic fitting tools (e.g., Visual DSD comparison, MATLAB-based curve fitting).
* **Human:** Molecular programming researchers (DNA circuit design), and chemical engineers (reaction modeling and calibration).

---

## When? (Temporal & Lifecycle Relevance)
* **Event/Trigger:** Occurs immediately upon system initialization ($t \approx 0$) when input strands interact with defective or partially formed gate complexes.
* **Defeater Frequency:** $k_{leak} \approx 1 \, \text{M}^{-1}\text{s}^{-1}.$ This is the second-order rate constant that quantifies the speed of unintended DNA strand displacement.
* **Phase/Lifecycle:** System preparation and initialization phase.

---

## Where? (Context and Scope)

* **System/Component:** DNA gate complexes and input strands.
* **Operational Context:** DNA strand displacement chemical reaction networks during system startup.

---

## How? (Mitigation & Response)

* **Monitoring & Mitigation:** Purify all DNA strands prior to assembly using PAGE or HPLC to remove truncated and misfolded species that contribute to unintended reactions. Introduce thresholding complexes that sequester spurious strand-displacement events before they propagate into downstream reactions. Track fluorescence deviation between expected and observed trajectories during the initial reaction window ($t \in [0, t_0]$)

* **Reliability and Validity:** Evaluation across independent experimental run $(n = 10)$ showed low inter-run variance in estimated initial leak. Fluorescence-based leak estimates and kinetic model–derived strand consumption showed agreement, with overlapping 95\% confidence intervals across methods and consistent batch-to-batch trends.

* **Limitations:** Thresholding introduces additional reactions that may alter system kinetics.

* **Residual Risks:** Even with fluorescence burst monitoring and baseline correction, very fast leak events may remain partially unobserved due to finite reporter response time, leaving a bounded underestimation of true initial depletion.

---

## Additional Comments

* **Notes:** Initial leak is a well-documented artifact in DNA strand-displacement systems and is typically treated as a preparation-induced deviation rather than explicitly modeled within the CRN abstraction.
