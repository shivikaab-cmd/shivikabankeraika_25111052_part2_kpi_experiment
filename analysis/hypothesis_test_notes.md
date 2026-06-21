# Hypothesis Test Notes

## Metric Being Tested

**Activation Rate** (Primary North Star Metric)

Activation Rate is defined as:

Activation Rate = Users who completed onboarding / Total users

This metric measures the effectiveness of the onboarding experience and indicates how successfully users progress through the activation journey.

---

## Reason for Choosing This Metric

The primary objective of the experiment is to determine whether the new onboarding and activation campaign improves user activation. Activation Rate is the most relevant metric because it directly reflects whether users complete the onboarding process and reach the desired activation milestone.

A higher Activation Rate indicates that the onboarding experience is more effective at guiding users toward successful product adoption, making it an appropriate metric for business decision-making.

---

## Null Hypothesis (H0)

The new onboarding experience does not improve Activation Rate compared to the existing onboarding experience.

**H0:** Activation Rate (Treatment) ≤ Activation Rate (Control)

---

## Alternative Hypothesis (H1)

The new onboarding experience improves Activation Rate compared to the existing onboarding experience.

**H1:** Activation Rate (Treatment) > Activation Rate (Control)

---

## Test Type

**One-Tailed Two-Proportion Z-Test**

A one-tailed test is appropriate because the business objective is specifically to determine whether the Treatment experience increases Activation Rate. The experiment is not testing for any difference in either direction; it is testing for improvement.

---

## Significance Level

**α = 0.05 (5%)**

The null hypothesis will be rejected if the p-value is less than 0.05.

---

## Test Inputs

| Metric                     | Control | Treatment |
| -------------------------- | ------- | --------- |
| Total Users                | 693     | 715       |
| Users Completed Onboarding | 108     | 152       |
| Activation Rate            | 15.58%  | 21.26%    |

---

## Statistical Test Results

| Measure                   | Value                   |
| ------------------------- | ----------------------- |
| Control Activation Rate   | 15.58%                  |
| Treatment Activation Rate | 21.26%                  |
| Difference                | +5.68 Percentage Points |
| Pooled Rate               | 18.47%                  |
| Standard Error            | 2.07%                   |
| Z-Score                   | 2.74                    |
| P-Value (One-Tailed)      | 0.003                   |

---

## Interpretation Logic

* If p-value < 0.05, reject the null hypothesis.
* If p-value ≥ 0.05, fail to reject the null hypothesis.
* A statistically significant result indicates that the observed improvement is unlikely to be due to random chance.

---

## Decision

The calculated p-value is **0.003**, which is lower than the significance level of **0.05**.

Therefore, the **null hypothesis is rejected**.

There is sufficient statistical evidence to conclude that the Treatment onboarding experience significantly improves Activation Rate compared to the Control onboarding experience.

---

## Business Interpretation

The Treatment group achieved an Activation Rate of **21.26%**, compared to **15.58%** for the Control group, representing a meaningful improvement in onboarding effectiveness.

The statistical test confirms that this improvement is significant and unlikely to have occurred by chance. Based on these results, the new onboarding experience demonstrates a positive impact on user activation.

Provided that guardrail metrics such as Refund Rate, Support Ticket Rate, and overall customer experience remain within acceptable limits, the company should consider rolling out the new onboarding experience to a broader user base.
