# -task4-Data-Storytelling-Statistical-Validation
## 📌 Executive Overview
This repository contains the complete deliverables for **Task 4: Data Storytelling & Statistical Validation**. The objective of this project is to synthesize data analytics findings into a structured business narrative and apply statistical hypothesis testing (Welch's Two-Sample T-Test) to validate whether a new website redesign layout leads to a statistically significant improvement in customer conversion rates.

---

## 🎯 Key Project Objectives
1. **Craft a Business Narrative:** Structure analytical findings into a cohesive story featuring problem context, analysis, statistical validation, and a clear call to action (CTA).
2. **Statistical Hypothesis Testing:** Formulate and execute an A/B testing framework to test the effectiveness of the new layout against the baseline control layout.
3. **Executive Presentation Deck:** Produce a visual, concise slide deck (`presentation_deck.pdf`) suitable for stakeholder presentations.
4. **Deliverable Package:** Provide documented python scripts, exported dataset summaries, and video outline guidelines.

---

## 📊 A/B Testing & Statistical Methodology

### 1. Hypothesis Formulation
* **Null Hypothesis ($H_0$):** $\mu_B - \mu_A = 0$  
  *(The new website layout has no effect on user conversion rates.)*
* **Alternative Hypothesis ($H_1$):** $\mu_B - \mu_A > 0$  
  *(The new website layout leads to a statistically significant increase in conversion rates.)*

### 2. Experimental Setup
* **Control Group (Group A - Old Layout):** $N = 100$ cohorts, Baseline Conversion Mean $ pprox 9.80\%$ ($\sigma = 2.0\%$).
* **Variant Group (Group B - New Layout):** $N = 100$ cohorts, Test Conversion Mean $ pprox 12.05\%$ ($\sigma = 2.0\%$).
* **Significance Level ($ lpha$):** 0.05 (95% Confidence Level).
* **Statistical Method:** Welch's Two-Sample Independent T-Test.

---

## 📈 Key Findings & Results Summary

| Metric / Parameter | Group A (Old Layout) | Group B (New Layout) | Impact / Test Result |
| :--- | :---: | :---: | :---: |
| **Sample Size ($N$)** | 100 cohorts | 100 cohorts | 200 Total Batches |
| **Mean Conversion Rate ($\mu$)** | **9.80%** | **12.05%** | **+2.25% Absolute Gain** |
| **Relative Lift** | — | — | **+22.96% Lift** |
| **T-Statistic ($t$)** | — | — | **$-7.8924$** |
| **P-Value ($p$)** | — | — | **$2.87 	imes 10^{-13}$** ($p < 0.05$) |
| **95% Confidence Interval** | — | — | **$[+1.69\%, +2.81\%]$** |
| **Statistical Decision** | — | — | **REJECT $H_0$** |

### Decision & Business Conclusion
With $p < 0.0001$ well below our $ lpha = 0.05$ threshold, we **Reject the Null Hypothesis ($H_0$)**. The observed increase in conversion rate is statistically significant and highly unlikely to be the result of random variation.

**Projected Financial Impact:**  
Full rollout across 100% of website traffic is projected to generate **+$140,000 in incremental revenue** annually.

---

## 📂 Repository File Structure

```text
.
├── hypothesis_testing.py          # Python script executing Welch's T-Test & summary logic
├── hypothesis_testing_results.csv # Tabular export of A/B test statistics and results
├── presentation_deck.pdf          # 6-Slide Executive Presentation Deck (A4 Landscape)
├── presentation_deck.html         # Source HTML styling template for PDF rendering
└── README.md                      # Project documentation and summary report
```

---

## 🚀 How to Run the Analysis

### Prerequisites
Ensure Python 3.8+ and required libraries are installed:
```bash
pip install numpy pandas scipy weasyprint
```

### 1. Execute Statistical Test Script
Run `hypothesis_testing.py` to calculate metrics and print terminal logs:
```bash
python hypothesis_testing.py
```

### 2. Generate PDF Presentation Deck
Run `weasyprint` to convert HTML template to PDF:
```python
from weasyprint import HTML
HTML('presentation_deck.html').write_pdf('presentation_deck.pdf')
```

---

## 🎥 Stakeholder Presentation Guide (LinkedIn Video Outline)
* **Duration:** 7–10 Minutes
* **Target Audience:** Product Managers, Executive Leadership, Marketing Stakeholders
* **Structure:**
  1. **Intro (1 min):** Project background, business dilemma, target goal (11.00%).
  2. **Data Story (2 mins):** User friction points identified on old checkout flow.
  3. **Statistical Testing (3 mins):** Walkthrough of $t$-test methodology, $p$-value interpretation, and $95\%$ confidence interval.
  4. **Recommendations & ROI (2 mins):** Full rollout strategy and $140k/year financial projection.
  5. **Q&A Closing (1 min):** Final takeaway and wrap-up.
