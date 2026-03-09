# Salary-in-football
⚽ Moneyball: The FIFA Edition
Does talent alone set your salary, or is it the jersey you wear?

Welcome to the financial autopsy of the "Beautiful Game"! This project dissects professional football salaries using the massive FIFA 21 dataset. We wanted to know: does your paycheck depend solely on your assists, or is playing striker for Real Madrid the ultimate financial "cheat code"?
🧐 The Mission

Led by a powerhouse research team, this study tackles a burning question: why do two players with similar stats often have vastly different bank accounts?

We put the following under the microscope:

    Performance: Overall ratings and clinical finishing ability.

    The Position Gap: Is a world-class goalkeeper financially "punished" compared to a goal-scorer? (Spoiler: Yes).

    The "Jersey Effect": The massive impact of club affiliation and market visibility on your weekly wage.

🛠️ The Tech Stack

To process over 18,000 players and 100+ variables, we brought out the heavy artillery in R:

    Data Wrangling: tidyverse, dplyr, and lubridate for time-series cleaning.

    Econometric Engine: Broom for sleek, tidy OLS regressions.

    Machine Learning (Robustness): glmnet for Elastic Net (Lasso + Ridge) to handle highly correlated player skills.

    Pro Reporting: knitr and XELATEX for high-quality PDF outputs.

📂 The Battle Plan (Workflow)

Our pipeline was built for precision, not just speed:

    1. The Big Scrub: We standardized currencies to Euros and physical units to CM/KG. Since match stats were missing, we engineered a "Goals" proxy using the Finishing attribute.

    2. The GOAT Alert: We identified extreme outliers early on. We actually had to exclude Lionel Messi from some visualizations because his salary was so astronomical it broke our charts!

    3. The OLS Laboratory: We ran three progressive models to isolate the pure effect of talent, then position, then the "club premium".

    4. Stress Testing: We used Elastic Net regularization to ensure our results weren't just statistical noise from overlapping skills.

📈 The Verdict: What We Found

    Overall is King: A one-point increase in your overall rating is associated with a 15% jump in weekly wages.

    The Striker Premium: At the exact same performance level, forwards earn 9–10% more than defenders.

    The Goalkeeper "Discount": Keepers suffer a substantial 15% wage hit compared to field players with similar ratings.

    The Club Factor: While elite clubs pay a massive premium, performance remains the absolute decider of who earns what inside the locker room.

🚀 Ready to Audit the Pitch?

    Get the Data: Ensure FIFA21.ods or FIFA21_Cleaned.csv is in your DATA folder.

    Ignition: Open mark final version.Rmd in RStudio.

    Knit: Compile the document to see the full report, including the boxplots and the "Superstar Effect" analysis.
