# 1. Business Problem Statement

## Overview

The company has launched a new onboarding and activation campaign to improve user conversion and early engagement. Users have been divided into two groups:

- Control Group: Existing onboarding experience
- Treatment Group: New campaign experience

The objective is to determine whether the new onboarding experience should be rolled out to all users.

## Decision to be Made

The key business decision is whether the treatment experience performs better than the existing onboarding experience and should be launched to the entire user base.

## Who the Decision Impacts

This decision impacts:

- New users joining the platform
- Product and Growth teams
- Marketing teams
- Business leadership and stakeholders
- Revenue and customer success teams

## Metric That Should Improve

The primary objective of the new onboarding campaign is to improve user conversion and early engagement.

Key metrics that should improve include:

- Activation Rate
- Conversion Rate
- User Engagement Rate
- Revenue per User

The treatment group should demonstrate a statistically significant improvement in these metrics compared to the control group.

## Risks That Must Be Monitored

While improving the primary KPI, the company must monitor:

- User retention
- Churn rate
- Revenue per user
- Customer satisfaction
- Other guardrail metrics

The campaign should not negatively affect these business outcomes.

## Evidence Required Before Recommendation

Before recommending a full rollout, the following evidence is required:

1. Comparison of KPI performance between control and treatment groups.
2. Statistical significance testing.
3. Evaluation of guardrail metrics.
4. Assessment of business impact.
5. Confidence that results are not caused by random variation.

The final recommendation will be based on both statistical evidence and business impact.

# Business Problem Summary

## Objective

Determine whether the new onboarding and activation campaign should be rolled out to all users.

## Decision Required

Leadership must decide whether the treatment group outperforms the control group and delivers meaningful business value.

## Success Metrics

The campaign should improve:

- Conversion Rate
- Activation Rate
- User Engagement
- Revenue Performance

## Risks

The company must monitor:

- Retention Rate
- Churn Rate
- Revenue Per User
- User Experience Metrics

## Evidence Needed

The recommendation will be based on:

- KPI comparison between groups
- Statistical significance testing
- Guardrail metric evaluation
- Business impact assessment

## Expected Outcome

If the treatment group demonstrates statistically significant improvements without negatively impacting guardrail metrics, a full rollout of the campaign should be recommended.


# 2. North Star Metric

## Selected North Star Metric: Activation Rate

### Why This Metric Is the Main Success Metric

Activation Rate is the percentage of users who successfully complete the desired onboarding actions and become active users. The primary objective of the new onboarding campaign is to improve early user engagement and encourage users to reach the activation stage more efficiently.

Since activation is the first meaningful step in the user journey, improvements in activation rate directly indicate whether the new onboarding experience is more effective than the existing experience.

### Why Other Metrics Are Supporting Metrics

Other metrics such as Conversion Rate, Revenue per User, Retention Rate, and Engagement Rate are important but are considered supporting metrics because they are outcomes that occur after activation.

A user must first become activated before they can generate revenue, remain engaged, or be retained over time. Therefore, these metrics help validate the overall impact of the campaign but do not serve as the primary success measure.

### How This Metric Connects to Business Growth

A higher Activation Rate means more users successfully adopt the product and begin experiencing its value. This increases the likelihood of:

- Higher conversion rates
- Improved customer retention
- Increased revenue generation
- Better customer lifetime value

As more users become activated, the company can achieve sustainable growth and stronger business performance.

### What Could Go Wrong If This Metric Is Optimized Blindly

Focusing only on Activation Rate may encourage actions that increase short-term activation but negatively affect the overall user experience.

Potential risks include:

- Users being pushed through onboarding too aggressively
- Lower user satisfaction
- Increased churn after activation
- Reduced long-term retention
- Lower revenue quality

For this reason, guardrail metrics such as Retention Rate, Revenue per User, and User Satisfaction should also be monitored when evaluating the success of the campaign.

# Recommendation Memo

## Executive Summary

An A/B test was conducted to evaluate a new onboarding and activation experience against the existing onboarding flow. The objective was to improve user activation while monitoring key guardrail metrics. Results show that the Treatment group significantly outperformed the Control group on activation-related metrics and revenue metrics. Although support ticket rates increased, overall business impact remains positive.

## North Star Metric

**Activation Rate (Onboarding Completion Rate)**

Activation Rate = Users who completed onboarding / Total users

Control: 15.58%

Treatment: 21.26%

Improvement: +5.67 percentage points

## KPI Tree Explanation

Business Goal → Increase Customer Activation and Revenue

- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate (North Star Metric)
- Paid Conversion Rate
- Revenue Per User

Guardrail Metrics:

- Refund Rate
- Support Ticket Rate
- Average Days to Convert
- Engagement Score

## Experiment Result Summary

| Metric | Control | Treatment | Difference |
|----------|----------|----------|----------|
| User Count | 693 | 715 | +22 |
| Landing Page Visit Rate | 63.64% | 72.59% | +8.95% |
| Trial Start Rate | 25.11% | 29.09% | +3.98% |
| Onboarding Completion Rate | 15.58% | 21.26% | +5.67% |
| Paid Conversion Rate | 3.17% | 6.99% | +3.82% |
| Revenue Per User | 51.75 | 53.88 | +2.13 |
| Engagement Score | 57.03 | 62.93 | +5.91 |
| Days to Convert | 8.86 | 6.40 | -2.46 |

The Treatment group consistently outperformed the Control group across key conversion and engagement metrics.

## Hypothesis Test Interpretation

A one-tailed proportion Z-test was performed on the Activation Rate.

- Control Rate = 15.58%
- Treatment Rate = 21.26%
- Z-Score = 2.74
- P-Value = 0.003
- Significance Level = 0.05

Since the p-value is less than 0.05, the null hypothesis is rejected. The new onboarding experience significantly improves user activation.

## Guardrail Analysis

### Refund Rate
- Control: 0.00%
- Treatment: 0.42%
- Risk Level: Low

### Support Ticket Rate
- Control: 14.72%
- Treatment: 24.76%
- Risk Level: Moderate

### Average Days to Convert
- Control: 8.86
- Treatment: 6.40
- Positive Impact

### Engagement Score
- Control: 57.03
- Treatment: 62.93
- Positive Impact

### Revenue Per User
- Control: 51.75
- Treatment: 53.88
- Positive Impact

Overall, guardrail metrics indicate positive business impact, although support ticket volume should be monitored.

## Segment-Level Insight

Region, Device Type, Traffic Source, and Plan Type distributions were balanced across Control and Treatment groups.

Key findings:

- Regional distribution remained consistent across groups.
- Mobile users represented the largest device segment.
- Traffic source distribution showed no acquisition bias.
- Plan type distribution was nearly identical across groups.

These results suggest successful experiment randomization and reliable treatment effects.

## Final Recommendation

### Launch

Recommendation: Launch the new onboarding experience to all users while closely monitoring support ticket rates.

Reasons:

- Statistically significant improvement in Activation Rate.
- Higher Paid Conversion Rate.
- Increased Revenue Per User.
- Improved Engagement Score.
- Faster Conversion Time.
- Low Refund Risk.

## Risks and Limitations

- Support Ticket Rate increased noticeably and may indicate onboarding friction.
- Experiment duration may not capture long-term retention behavior.
- Revenue quality should continue to be monitored after rollout.

## Next Steps

1. Roll out the new onboarding experience gradually.
2. Monitor support ticket volume closely.
3. Track retention and revenue quality post-launch.
4. Conduct follow-up experiments to optimize onboarding support content.
5. Continue monitoring guardrail metrics after deployment.


