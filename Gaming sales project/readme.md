# Codecademy Final Portfolio Project 2
## Ryan Cheung

### topic 2: Video Game sale data

## GOALS:
In this project, I want to explore the performances and ratings and interactions of various real life factors that influence the performance of a game in the eyes of a critical audience versus their performance in the market. 

1. How have global video game sales shifted across regions (NA, EU, JP, Other) over time?

    Reason: Reveals market expansion/contraction and shifting consumer bases (e.g., rise of Asia, decline of Japan’s relative share).

2. Which genres consistently outperform others in each major region (NA, EU, JP)?

    Reason: A publisher could tailor its portfolio regionally (e.g., RPGs for Japan, shooters/sports for NA/EU)

3. Is there a correlation between critic score (Critic_Score) and global sales? Does this relationship differ by genre or platform?

    Reason: Tests the real-world impact of reviews. You can also compare User_Score vs. critic score.

4. What is the distribution of User_Score vs. Critic_Score? Are there games where these diverge widely (“critic darlings” vs. “fan favorites”)?

    Reason: Identifies controversial or underrated/overrated titles – a great storytelling hook.

5. How many years does it typically take for a new gaming platform to reach its peak sales? Which platforms had the longest/shortest lifecycles?

    Reason: For hardware manufacturers, understanding platform longevity informs R&D and marketing.

6. Which publishers are most dominant in each genre? (“Genre specialists” vs. “generalists”)

    Reason: Reveals strategic positioning – e.g., Nintendo owns Platform/Sports, Take-Two dominates Action.


7. What is the relationship between a game’s Rating (ESRB: E, E10+, T, M) and its sales in different regions? Does M-rated games sell better in NA vs. JP?

    Reason: Cultural differences in acceptance of mature content affect localization and marketing.

8. Are there “hidden gems” – games with high critic scores but very low global sales? Which developers create consistently high-quality niche titles?

    Reason: For investors or publishers looking for acquisition targets or underserved markets.

## DATA:
Video Game data was grabbed from a Kaggle Dataset: https://www.kaggle.com/datasets/ibriiee/video-games-sales-dataset-2022-updated-extra-feat

## ANALYSIS / CONCLUSIONS

From the analysis, I have discovered that the modern gaming market is highly dynamic, segmented by geography, contains critically accalimed qualiry, and specialized development strategies. Success in this field requires a multi-pronged approach to capitalize on both mass appeal and untapped niches.

1. market dynamics:

- Global Volume Leader: North America has historically driven the largest absolute sales volume across all regions, with significant peaks around 2006.


- Shifting Center of Gravity: While NA maintains high overall numbers, Europe's market share dominance increased significantly post-1995, suggesting a sustained shift in global consumer base power away from Japan (which peaked earlier and showed relative decline).

- Regional Strategy Implication: A successful publisher must tailor its content mix to the current regional market leader. For example, capitalizing on Europe's growing share is key for future growth projections.

 2. Genre & Platform Strengths 

- Core Pillars: The genres of Sports, Action, and Platform remain global revenue pillars, consistently generating the highest total sales volumes across NA, EU, and JP. These should form the foundation of any large-scale content portfolio.

- Regional Specialization: Genres show clear regional preferences:

    - Japan: Exhibits a profound, enduring affinity for Role-Playing Games (RPGs).

    - North America & Europe: Show balanced strength across Action/Sports, but the market is less genre-locked than Japan's.

- Strategic Tool: Simple sales figures are insufficient; understanding normalized metrics like the Regional Contribution Indices (RCI) and Cross Regional Ratios is crucial for accurate global planning.

3. The "Hidden Gem" Opportunity
- The Undervalued Asset: The most critical finding is the existence of the "hidden gem"—titles with high critical scores ( >= 85) but low commercial sales. This proves that critical quality does not equate to immediate mainstream sales, creating a significant market opportunity for discovery and promotion.

- Targeting Niche Talent: The top 10 developers identified are reliable sources of this high-quality niche content. These studios represent the highest value assets for potential acquisition or strategic partnership.