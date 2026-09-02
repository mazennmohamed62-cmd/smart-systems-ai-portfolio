# Voice Card & Framed Case Study

## Voice Card
* **Tone & Rules:** Direct, hands-on engineer, plain-spoken, no buzzwords. Focus on real system metrics, explicit design trade-offs, and clear operational outcomes.

---

## Case Study: Predictive Maintenance in Industrial IoT (Machine Learning Track)

### 1. The Problem
Industrial machines on assembly lines fail unexpectedly, causing costly factory downtime and damaged hardware. Static threshold rules (e.g., "alert if temperature > 80°C") fail because they ignore multi-sensor signals (like subtle vibration increases under normal heat) and trigger too many false alarms that field technicians end up ignoring.

### 2. What I Did & Decided
I framed failure prediction as a binary classification task to flag high-risk nodes 24 hours ahead. I audited sensor signals to confirm that temperature instability and vibration RMS are reliable leads, encoded an explicit baseline rule, and then trained a Random Forest model. I prioritized high Recall with an 85%+ Precision constraint so field teams only get dispatched when an intervention is actually warranted.

### 3. What Came Of It
The ML model improved failure detection recall by +30% compared to static rules while cutting false alarms. The system outputs an actionable dispatch queue (`SCHEDULE_EMERGENCY_INSPECTION`) saved as `baseline_action_score.csv` alongside verified system performance metrics in `w05_metrics.json`.

---

## Before / After Copy Comparison

* **Generic AI Draft (Before):**
  > "Leveraged cutting-edge Machine Learning and advanced IoT telemetry to deliver a robust, results-driven predictive maintenance solution that optimizes operational efficiency and prevents critical system failures."

* **Edited Version (After):**
  > "Trained a Random Forest model on temperature and vibration telemetry to catch machine failures 24 hours early—improving detection by 30% over static rules without flooding technicians with false alerts."
