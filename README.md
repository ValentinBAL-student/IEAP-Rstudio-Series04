# IEAP RStudio - Series 04: Regression, Noise & Heart Rate Recovery Modeling

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/ValentinBAL-student/IEAP-Rstudio-Series04)
[![Language-R](https://img.shields.io/badge/Language-R-276DC3?logo=r)](https://www.r-project.org/)
[![Quarto-Typst](https://img.shields.io/badge/Output-Quarto%20%7C%20Typst%20PDF-brightgreen)](https://quarto.org/)

This repository contains the code, data, analytical reports, and one-page synthesis for **Series 04**, investigating the effects of stochastic noise on linear regression and fitting non-linear mathematical models to post-exercise heart rate recovery (HRR) data.

---

## 👥 Team Members & Division of Labor

| Member | Primary Responsibilities & Contributions |
| :--- | :--- |
| **BALBINE Valentin** | **Task 2: Noise in Linear Regression**<br>• Designed synthetic datasets across 3 noise levels ($\sigma = 1, 4, 10$).<br>• Model fitting with `lm()`, parameter extraction ($\hat{\beta}, \text{SE}, R^2, \text{RMSE}$).<br>• Formulated prior expectations and proposed Monte Carlo protocol improvements. |
| **TUBA Tuba** | **Task 3: Heart Rate Recovery (HRR) Modeling**<br>• Literature review on autonomic physiological mechanisms (vagal vs. sympathetic phases).<br>• Data exploration and preprocessing of Aidlab telemetry (peak detection, $t=0$ cropping).<br>• Non-linear model fitting (Linear, Mono-exponential, Bi-exponential) via `nlsLM`. |
| **LONG Jiangbin** | **Synthesis, Conclusions, Repository & PDF Report**<br>• Synthesized overall discussion and physiological parameter interpretation.<br>• Managed GitHub repository architecture, version control, and documentation.<br>• Designed and compiled the strict one-page critical reflection report using Quarto & Typst. |

---

## 📂 Repository Structure

```text
.
├── README.md                  # Project overview, team division, and documentation
├── one_page_report.qmd        # Source code for the 1-page critical reflection (Typst PDF)
├── one_page_report.pdf        # Compiled 1-page PDF document for final submission
├── task2_noise_simulation/    # Scripts and analysis for Task 2 (Linear regression & noise)
│   ├── task2_simulation.R    # Synthetic data generation and lm() model fitting
│   └── task2_plots.png        # Comparative regression and residual plots
├── task3_hr_recovery/         # Scripts and analysis for Task 3 (Aidlab HRR modeling)
│   ├── task3_analysis.qmd     # Complete R code, nls fits, metrics table, and discussion
│   └── data/                  # Aidlab physiological recordings (3-hour & 7.5-min datasets)