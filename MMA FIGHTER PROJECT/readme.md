# Codecademy Final Portfolio Project 1
#### Ryan Cheung

### topic 1: MMA fighter data

## GOALS:

In this project, I want to explore the dynamics of an MMA fight, using data analysis techniques to identify and display the various factors that influence a fighter's victory or loss.

### Theme 1: Predictive Modelling & Key Win Factors
- 1: Which single-round metric is the strongest predictor of victory?
    - Reason: Wins and Losses are the ultimate outcome of a fight. We can compare if landing more significant strikes, takedowns, control time, or knockdowns is the most effective predictor.

- 2: Is it possible to predict the method of victory based on a fighter's attributes before the match and during early rounds?
    - reason: We move beyond the win / loss itself into *how* the fight ends. (KO, TKO, submissions, decision)

- 3: Does a fighter's win streak, age, and weight class ('stock') correlate with in-round aggression?
    - Reason: tests if winning fighters take more risks or become more efficent

### Theme 2: Round-by-Round Dynamics & Comebacks
- 4: What statistical patterns differentiate fighters who win the fight after losing the 1st round vs those who don't?
    - Reason: quantifies adjustments and 'guts'. Filter for fights where the winner actually lost in round 1, and compare to rounds 2-3. take this and compare to the loser of this particular match.

- 5: How does the striking target (head vs body vs legs) chagne from ruond 1 to round 3, and does this shift correlate with a win?
    - Reason: analyze the efficacy of various fight strategies (slow down movement with leg kicks, body shots to drain stamina, head strikes for the KO, etc...)

### Theme 3: Fighter Profiling & Style Clustering
- 6: Can we identify distinct 'fighter archetypes' based on round-y-round striking / takedown ratios and control times?
    - Reason: use K means Clustering to make fighter profiles, and analyze what archetypes win most often, or what archetype beats what.

- 7: Do fighters who rely on leg kicks win more often, or do the tend to lose later rounds as the leg kicks accumulate?
    - Reason: tests the leg kick theory, where reducing opponent mobility is worth risk of counters.

### Theme 4: Contextual Factors & Anomalies
- 8: Does hometown advantage actually matter?
    - Reason: classic real world bias tests.

- 9: which weight class has the highest rate of 1st round finishes, and what striking / takedown metrics drive this?

-10: do taller fighters with a reach advantage control distance better?
    - Reason: test a fundamental striking concept.

## DATA:

MMA Fighter data grabbed from kaggle.com: https://www.kaggle.com/code/rishpande/ufc-data-analysis-visualization-beginner

## ANALYSIS / CONCLUSIONS:
