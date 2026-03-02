Team: The Outliers

# Deep-Kitchen KPT Engine

### *Precision ETA via 18-Signal Enrichment & Merchant De-biasing*

## ⚡ The Quick Pitch

Standard KPT models are "blind" to the internal chaos of a kitchen. They rely on **Biased Merchant Signals** (FOR button), leading to riders waiting idly. We built a **Digital Twin** that models kitchen physics to predict the *real* handover time.

## 📊 Proprietary Dataset

* **Scale:** **31,000+ Unique Orders** (Self-curated for high variance).
* **Feature Depth:** **18 Custom Signals** (Environmental + Psychological + Physical).
* **Data Integrity:** Chronological sorting to ensure **Zero Data Leakage**.

## 🛠 The 18-Signal Architecture (The "Juicy" Part)

### 🧩 Layer 1: The "Hidden" Stress Signals

* **WiFi Crowd Proxy:** Uses signal strength to "see" dine-in customers Zomato misses.
* **Rush Window Bucket:** Live ratio of order velocity vs. kitchen bandwidth.
* **Pending Queue:** Real-time backlog tracking of the live kitchen stack.

### 🧠 Layer 2: The "Chef Psychology" Signals

* **Context-Switch Penalty:** (**Our Innovation**) Measures the cognitive delay when a chef switches between diverse dish types.
* **Instruction Friction:** NLP-derived index for "Customization" keywords that break kitchen rhythm.
* **Packaging Complexity:** Scoring based on dish state (Liquids/Gravies require +X mins for sealing).

### 🌍 Layer 3: Geospatial & Atmospheric Signals

* **Vertical Transit Cost:** Predicts the "Mall Floor Delay"—time spent in elevators/stairs.
* **Weather Impact:** Humidity and Rain intensity factored into frying times and hand-off friction.

### ⚓ Layer 4: The Anchor Signals

* **Past KPT Baseline:** 30-day "Normal" anchor for specific store/time slots.
* **Merchant Reputation:** A de-biasing score to penalize "Early-Button Clickers."

## 🚀 Performance Metrics

*Optimized via **Tuned CatBoost** & Validated with **5-Fold Rolling Time-Series CV**.*

| Metric | Zomato Baseline | Our Enriched Model |
| --- | --- | --- |
| **MAE (Minutes)** | ~3.55 min | **~3.14 min** |
| **Reliability** | Fails during Rush | **Stable & Consistent** |
| **Error Reduction** | 0.00 min | **11.57% Improvement** |

## 💰 Business Impact (At 100k Daily Orders)

* **Fleet Efficiency:** **~685.07 Rider Hours/Day** reclaimed from idle waiting.
* **Rider Experience:** Massive reduction in "Gate Waiting" time.
* **Customer UX:** Hotter food delivery through precision dispatching.

---

**"We don't just predict the time; we model the friction."**
