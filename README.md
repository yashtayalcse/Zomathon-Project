Team: The Outliers

### **Zomathon 2026: The "Deep-Kitchen" KPT Framework**

**Precision ETA via 18-Signal Enrichment & Merchant De-biasing**

---

#### **1. Executive Summary: The Core Problem**

Standard Kitchen Prep Time (KPT) models fail due to **Merchant Signal Noise**. To avoid late-delivery penalties, merchants often click the "Food Ready" (FOR) button prematurely.

* **The Result:** Riders are dispatched too early, leading to idle waiting at the gate.
* **The Cost:** Thousands of fleet-wide rider-hours are lost daily.
* **The Blindspot:** Traditional systems lack visibility into **Dine-in Load** (offline customers) and internal kitchen friction.

---

#### **2. The Proprietary Dataset**

*Unlike baseline models, this framework is trained on a high-fidelity "Digital Twin" of Zomato’s kitchen clusters:*

* **Scale:** **31,000+ Unique Orders** (Custom-engineered for high variance).
* **Dimensionality:** **18 Intelligence Signals** capturing environmental, psychological, and physical friction.
* **Data Integrity:** Chronologically sorted to ensure **Zero Data Leakage**.

---

#### **3. The 18-Signal Intelligence Architecture**

We move beyond simple history by modeling **Kitchen Physics** through four specialized layers:

**A. Real-Time "Hidden" Load**

* **Dine-in Crowd Proxy:** WiFi sensing signals to detect non-Zomato customers in the vicinity.
* **Rush Window Bucket:** A dynamic ratio of live order volume vs. active chef capacity.
* **Pending Queue:** Real-time backlog tracking of the live kitchen stack.

**B. Operational & Psychological Friction**

* **Context-Switch Penalty:** (**Our Innovation**) Measures the cognitive delay caused by chefs switching between diverse dish types.
* **Packaging Complexity:** Scoring based on dish state (e.g., liquids/gravies require spill-proof sealing time).
* **Instruction Friction:** NLP-derived index scanning for high-effort "Special Instructions."

**C. Geospatial & Atmospheric Signals**

* **Vertical Transit Cost:** Models the "Mall Floor Delay"—time spent in elevators or stairs for high-rise restaurants.
* **Weather Impact:** Humidity and Rain intensity factored into cooking speed and handover friction.

**D. Merchant Trust Layer**

* **Past KPT Baseline:** 30-day "Normal" anchor for specific store/time slots.
* **Merchant Reputation:** A de-biasing score to penalize "Early-Button Clickers" based on historical trends.

---

#### **4. Model Performance & Evaluation**

We utilized a **Tuned CatBoost Regressor** for its symmetric tree stability and superior handling of categorical data (Store IDs).

| Metric | Baseline (Merchant Signal) | Our Enriched Model | % Improvement |
| --- | --- | --- | --- |
| **MAE (Minutes)** | ~3.50 min | **~2.20 min** | **~37%** |
| **Peak Reliability** | Spikes during Rush | **Stable & Reliable** | **+25% Accuracy** |

* **Tuning:** Optimized via `RandomizedSearchCV` for L2 Regularization.
* **Validation:** Verified through **10-Fold Rolling Time-Series Cross-Validation**.

---

#### **5. Business Impact (Scaled to 100k Daily Orders)**

* **Fleet Efficiency:** **~685.07 Rider Hours/Day** reclaimed from idle waiting.
* **Efficiency Gain:** **0.41 minutes** average reduction in error per order.
* **Strategic Outcome:** Higher "Trips per Hour" for riders and a significant reduction in "Cold Food" complaints due to precision dispatching.

---

**"We don't just predict the time; we model the friction."**
*Submission for Zomathon 2026 | Problem Statement 1 | Team Yash*
