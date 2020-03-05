# A/B Test Experiments

## Thorough Experiment with Confidence Interval, p-value for A/B test
* This is a typical A/B test problem.
### [My code][1]
* Online calculators can be used
  * Estimate sample size: https://www.evanmiller.org/ab-testing/sample-size.html
    * Given Type 1 error rate α, type II error rate β, basedline conversion rate, min detectable effect
  * Estimate p-value for binomial distribution: https://www.graphpad.com/quickcalcs/binomial1/
    * Given number of success, total trails, probability of success in biomial distribution
### Overall Process
1. Choose invariant metrics and evaluation metrics.
2. Estimation of baselines and Sample Size
  * Estimate population metrics baseline
  * Estimate sample metrics baseline
  * Estimate sample size for each evaluation metrics, only keep the metrics that have practical amount of sample size.
3. Verify null hypothese - Control Group vs. Experiment Group
  * Sanity check with invariant metrics
  * Differences in evaluation metrics, using confidence interval, Dmin to check both statistical, practical significance.
  * Differences in trending, using p_value to check statistical significance.


[1]: https://github.com/hanhanwu/Hanhan_Data_Science_Practice/blob/master/Applied_Statistics/ABTest_Experiments/detailed_ABTest_Experiment.ipynb