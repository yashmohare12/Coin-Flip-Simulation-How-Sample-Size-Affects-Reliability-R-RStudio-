# Coin Flip Simulation How Sample Size Affects Reliability using  R-RStudio 

Small samples can mislead; large samples reveal the true pattern, as long as the data is collected fairly
Coin Flip Simulation: How Sample Size Affects Reliability (R / RStudio)


<img width="684" height="706" alt="Rplot01" src="https://github.com/user-attachments/assets/d4284508-f557-420c-89df-090b02505fd2" />

*2. Probability vs. experimental result*
- Probability is what we expect in theory (heads = 1/2).
- The experimental result is what we actually observe from flips.

*3. Law of large numbers*
- The more times you repeat an experiment, the closer your result gets to the true probability.
- Your running-proportion plot showed this: it swings early, then settles near 0.5.
- It does not mean tails are "due" after a streak of heads. The coin has no memory.
- 
<img width="1426" height="874" alt="Rplot" src="https://github.com/user-attachments/assets/4b07404e-abba-428c-9bfc-652ebf3d4151" />

*4. Effect of sample size*
- n = 10: results spread widely (about 0.2 to 0.8).
- n = 100: more stable (about 0.4 to 0.6).
- n = 1000: very stable (about 0.47 to 0.53).
- The probability stays 0.5, but the reliability of your result improves.

*5. Key rule*
- More data = less luck = more trustworthy result.
- To get twice the precision, you need about 4 times the data.

*6. Real-life uses*
- A/B testing on websites
- Surveys and polls
- Insurance and casinos
- Companies like Netflix and Amazon using large datasets

*7. Limits to remember*
- Large data does not fix biased data.
- Returns shrink as data grows, so more is not always worth the cost.

*8. R skills practised*
- Installing and loading packages (install.packages, library)
- Simulating data with rbinom()
- Plotting with ggplot2 (geom_line, geom_histogram, facet_wrap)
- Fixing errors (package names, typos such as labeller)

*9. Final conclusion*
> Small samples can mislead; large samples reveal the true pattern, as long as the data is collected fairly.

*Next steps*
- Try an unfair coin: rbinom(5000, 1, 0.7).
- Do Part 3, the A/B test, to see how much data is enough.
