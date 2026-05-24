This is the strategy guide presented by opencode.

📊 Analysis Strategy: MMA Fighter Dynamics
Phase 1: Feature Engineering & Metric Mapping
Before answering any specific goal, the following derived metrics must be calculated across all available rounds (Round 1 through Round N) for each fighter (B_ID):

Derived Metric	Calculation Basis	Relevant Columns	Purpose
Total Aggression Score	Sum of 
All Strikes Landed
All Strikes Landed across all rounds.	All B__RoundX_...Landed columns	Measures overall fight activity and effectiveness.
Dominant Strike Ratio (DSR)	
Head Strikes
+
Body Strikes
Total Strikes Landed
Total Strikes Landed
Head Strikes+Body Strikes
​
 	B__RoundX_Strikes...	Identifies fighters who favor head/body attacks vs. total striking power.
Grappling Dominance	
Takedowns Landed
Takedowns Attempted
Takedowns Attempted
Takedowns Landed
​
 	B__RoundX_Grappling...	Measures success rate on the ground game.
Leg Kick Efficiency (LKE)	
Total Leg Kicks Landed
Total Strikes Landed
Total Strikes Landed
Total Leg Kicks Landed
​
 	All B__RoundX_Strikes_Clinch/Distance...	Quantifies reliance on leg kicks relative to total striking output.
Phase 2: Goal-Specific Analysis & Visualization Plan
Goal #	Goal Description	Key Columns Used	Feature Engineering Needed	Suggested Visualization
1	Strongest predictor of victory?	B_Weight, All 
Landed
Landed columns, Win/Loss Outcome.	Calculate average Total Aggression Score for KO vs TKO vs Decision outcomes.	Bar Chart: Average total landed strikes grouped by outcome category. (Tests if striking or grappling leads to higher overall output).
2	Predict win method?	BStreak, B_Age, 
Round 1
Round 1 Metrics, Outcome Type.	Calculate R1 Grappling/Striking ratio and compare this initial performance profile against the eventual outcome (KO/TKO/etc.).	Heatmap: Correlation matrix showing 
R1 Attempts
R1 Attempts vs. Win Type (e.g., high takedown attempt rate in R1 
→
→ TKO).
3	Streak, Age, Weight vs Aggression?	BStreak, B_Age, B_Weight, Total Aggression Score.	Calculate a composite aggression score and analyze its variance based on streaks/age bands within weight classes.	Scatter Plot: 
B_Age
B_Age (X-axis) vs. Mean Aggression Score (Y-axis), colored by BStreak category.
4	R1 Loss 
→
→ Win Pattern?	
Round 1
Round 1 Metrics, 
Round 2/3
Round 2/3 Metrics, Outcome Type.	Calculate the difference (
Δ
Δ) in key metrics (e.g., 
Strikes Landed
Strikes Landed) between Round 1 and later rounds for winners who lost R1 vs. others.	Comparative Bar Chart: Side-by-side comparison of 
Δ
Δ Striking/Grappling Stats for the two groups.
5	Striking Target Shift?	All Head/Body/Leg Strike columns across all rounds.	Calculate the percentage contribution of each target (Head, Body, Leg) in R1 vs. R3.	Grouped Bar Chart: Percentage distribution of striking targets over time (R1 vs R3).
6	Fighter Archetypes?	All 
Landed
Landed columns; B_Weight.	Standardize and normalize ratios like 
Takedowns Landed
Takedowns Attempts
Takedowns Attempts
Takedowns Landed
​
  for all fighters. Run K-means clustering on these normalized metrics.	Scatter Plot/Cluster Visualization: Points colored by cluster ID, with labels showing the primary defining characteristics of each archetype (e.g., "Striker," "Wrestler").
7	Leg Kick theory?	All B__RoundX_Strikes_Clinch/Distance metrics; Outcome Type.	Calculate LKE for all fighters and compare its distribution between winning vs losing groups.	Box Plot: Comparison of the Interquartile Range (IQR) of LKE values for winners vs. losers.
8	Hometown Advantage?	B_HomeTown, Win/Loss Outcome.	Group data by 
B_HomeTown
B_HomeTown and calculate win rates (
Wins
Total Fights
Total Fights
Wins
​
 ).	Bar Chart: Win Rate (%) per Home Town.
9	Weight Class & R1 Finishes?	B_Weight, Round 1 Outcome, R1 Metrics (Grappling vs Striking).	Filter for KO/TKO wins in R1. Compare the average 
Strikes Landed
Strikes Landed (striking) and 
Takedowns Landed
Takedowns Landed (grappling) across weight classes that excel here.	Doughnut Chart: Proportion of R1 finishes by Weight Class, supplemented by a bar chart showing which metric is dominant for each group.
10	Height/Reach Advantage?	B_Height, 
Distance Strikes Landed
Distance Strikes Landed columns; Total Striking.	Calculate correlation between 
B_Height
B_Height and the ratio 
Total Distance Strikes Landed
Total Strikes Landed
Total Strikes Landed
Total Distance Strikes Landed
​
 .	Scatter Plot: 
Height
Height (X-axis) vs. Avg Distance Strike Ratio (Y-axis), with a regression line showing positive/negative correlation.

