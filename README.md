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
