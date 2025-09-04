# From Consumers to Creators: Undergraduate-Created OERs

**Authors:** Natasha et al.  
**Date:** 2025-09-03 

> A pre–post activity study (n = 57) in an advanced biochemistry course evaluating whether creating OER improves **Creative Commons knowledge**, **perceptions of OER**, and **ability to access OER**.

---

## 🔎 Abstract

Open Educational Resources (OER) are growing across Canadian institutions. We assess whether involving undergraduates in **creating** OER improves (1) understanding of open licensing, (2) perceptions of OER credibility/utility, and (3) independent access behaviors. Using structured pre/post surveys and the **Wilcoxon Signed-Rank Test**, we observe significant gains in open-licensing knowledge (p < 0.001), credibility perceptions (p = 0.0049), and modest improvements in access behaviors (p = 0.0397). Thematic analyses reinforce these gains and point to needed institutional scaffolding for access.

---

## 🗂️ Repository Structure

```text
.
├─ data/
│  └─ Pre_Post_Survey.xlsx         # Sheets: "PreSurvey", "PostSurvey"
├─ scripts/
│  ├─ 01_load_and_clean.R          # Load data, convert blanks -> NA
│  ├─ 02_missingness_plots.R       # VIM::aggr for pre/post
│  ├─ 03_filter_high_missing.R     # Drop items with >20% missing (pre or post)
│  ├─ 04_long_format.R             # Pivot to long; combine pre/post
│  ├─ 05_descriptive_plots.R       # Faceted bar plot of Likert responses
│  ├─ 06_wilcoxon_all_items.R      # Paired Wilcoxon per item; volcano plot
│  ├─ 07_thematic_CC_licenses.R    # Theme 1: Q10–Q12 (boxplots + tests)
│  ├─ 08_thematic_perception.R     # Theme 2: Q6, Q15_CCS, Q15_FUR
│  └─ 09_thematic_access.R         # Theme 3: Q1_b_ii
├─ outputs/
│  ├─ Missing_Data_PreSurvey.png
│  ├─ Missing_Data_PostSurvey.png
│  ├─ Comparison_Pre_Post_Survey.png
│  ├─ volcano_plot_wilcoxon.png
│  ├─ Thematic_1_wilcoxon.png
│  ├─ Thematic_2_wilcoxon.png
│  └─ Thematic_3_wilcoxon.png
├─ README.md                        # (this file)
└─ analysis.Rmd                     # Optional end-to-end R Markdown
