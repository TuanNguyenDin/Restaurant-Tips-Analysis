# 🍽️ Restaurant Tips Analysis

Project Title: Restaurant Tips Analysis

Brief description:
This repository contains an exploratory data analysis of a restaurant "tips" dataset. The analysis inspects which factors influence tip amounts (for example: smoker status, gender, day of week, time of day) and demonstrates visualization techniques (histograms, boxplots, comparative plots) to summarize the findings.

Data description:
- **Source:** CSV used in the notebook is loaded from: `https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv`.
- **Dataset:** 244 observations of restaurant bills. Each row represents a single bill/tip record and includes the following columns:
	- `total_bill` : total bill amount (numeric)
	- `tip` : tip amount (numeric)
	- `sex` : sex of the payer (Male/Female)
	- `smoker` : smoker status (Yes/No)
	- `day` : day of the week (Thur, Fri, Sat, Sun)
	- `time` : time of day (Lunch/Dinner)
	- `size` : party size (integer)

How to access the data:
- The notebook loads the dataset directly from the raw GitHub URL above. If you prefer to download manually, open the URL in a browser and save the CSV, or run the notebook which reads the CSV from that URL.

Main goals:
- Explore distributions of tip values and compute descriptive statistics (min, max, mean, median).
- Compare tip behavior across groups: smokers vs non-smokers, male vs female, weekdays vs weekends, lunch vs dinner.
- Visualize distributions and outliers using histograms and boxplots.

Results / Main findings:
- **Smoker vs Non-smoker:** Smokers tend to have slightly higher mean and median tip values. The smoker group includes a few very large tips that increase central tendency measures.
- **Gender:** Males show a slightly higher average tip and produce more of the extreme (very large) tip values — the distributions for both sexes are concentrated around 2–4, but males have a longer tail of large tips.
- **Weekday vs Weekend:** Weekends (Saturday and Sunday) tend to bring higher median tips and show a greater spread and more high-value tip outliers compared to weekdays.
- **Lunch vs Dinner:** Dinner shifts the distribution toward higher tips (higher median and more large-tip outliers) compared to lunch.

Key visualizations and where to find them:
- All visualizations (histograms, combined charts, and boxplots) and step-by-step calculations are provided in the Jupyter Notebook: `Restaurant_tips_analysis.ipynb`.
- The notebook also includes a Colab badge for one-click opening in Google Colab.

How to run the analysis locally:
1. Install the required Python packages (if needed):

```
pip install pandas numpy seaborn matplotlib
```

2. Open `Restaurant_tips_analysis.ipynb` in Jupyter Notebook, JupyterLab, or upload/open it in Google Colab (Colab link in the notebook). Run the cells in order — the notebook reads the data from the URL and recreates the analysis and plots.

Notes and next steps:
- The notebook contains the full exploratory workflow, including type corrections, descriptive statistics, grouped comparisons, and plotting code.
- If you want a script version or to export the figures as image files, I can add a `requirements.txt` and a small Python script to reproduce key charts automatically. Would you like me to add that?

