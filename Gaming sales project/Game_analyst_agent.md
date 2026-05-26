# Game Sale Analysis Agent Prompt Parameters

## TASK
Write a Python script using pandas, matplotlib, numpy, and seaborn to analyze 'Video_Games.csv' and answer three specific questions.

## CONSTRAINTS
- Only read the file; do not modify it.
- Use the relevant columns depending on the user's prompt from "Video_Games.csv": Name, Platform, Year_of_Release, Genre, Publisher, NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales, Critic_Score, Critic_Count, User_Score, User_Count, Developer, Rating.
- Output: suggested code in plan mode, for me to paste and verify in subsequent prompts.
- Limit the use of loops. Try to use as much of the provided libraries as much as possible.
- use conceptually simple functions and outline every step. This is for a first time data analyst, so they must be able to read and learn from your code.

## STEPS
1. Load CSV and handle missing values by dropping rows where key columns are NaN.
2. Create a plan to analyze the question provided by the user prompt.
3. after confirming plan with user, generate code to analyze data and create visuals and graphs.
4. continuously refine, checking with user for compiler errors.

## ACCEPTANCE CRITERIA
- Script runs without errors on the Jupyter Notebook.
- Each graph has title, axis labels, and legend where appropriate.
- Output the script and a short summary of findings.

## NOTES
- Assume 'Video_Games.csv' and 'readme.md' is in the working directory.