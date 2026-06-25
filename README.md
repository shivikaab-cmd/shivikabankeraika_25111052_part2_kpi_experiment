# KPI Experiment Analysis – A/B Testing Project

## Author Information

**Name:** Shivika Bankeraika
**Student ID:** bitsom_ba_25111052

---

# 1. Business Context

A subscription-based product company tested a new onboarding and activation campaign against the existing onboarding experience. The goal was to determine whether the new onboarding flow improves user activation and downstream business outcomes while maintaining acceptable customer experience metrics.

The experiment compared:

* **Control Group:** Existing onboarding experience
* **Treatment Group:** New onboarding and activation campaign

The business decision was whether to launch the new onboarding experience, continue testing, or reject the change.

---

# 2. Dataset Description

The dataset contains user-level experiment data with the following key variables:

| Variable             | Description                           |
| -------------------- | ------------------------------------- |
| user_id              | Unique user identifier                |
| signup_date          | User signup date                      |
| experiment_group     | Control or Treatment                  |
| region               | User region                           |
| device_type          | Desktop, Mobile, Tablet               |
| traffic_source       | Acquisition channel                   |
| plan_type            | Subscription plan                     |
| visited_landing_page | Landing page visit indicator          |
| started_trial        | Trial start indicator                 |
| completed_onboarding | Onboarding completion indicator       |
| converted_to_paid    | Paid conversion indicator             |
| revenue_30d          | Revenue generated within 30 days      |
| support_tickets_30d  | Support tickets raised within 30 days |
| refund_requested     | Refund indicator                      |
| days_to_convert      | Days required to convert              |
| engagement_score     | User engagement score                 |

Total Users: **1,408**

* Control: **693**
* Treatment: **715**

---

# 3. North Star Metric Selected

## Activation Rate (Onboarding Completion Rate)

Activation Rate = Users who completed onboarding ÷ Total users

This metric was selected because the primary purpose of the new onboarding campaign is to improve user activation. Higher activation is expected to positively influence retention, engagement, and revenue generation.

Results:

| Group     | Activation Rate |
| --------- | --------------- |
| Control   | 15.58%          |
| Treatment | 21.26%          |

Improvement: **+5.67 percentage points**

---

# 4. KPI Tree Summary

Business Goal: Increase User Activation and Revenue

### Primary KPI

* Activation Rate (North Star Metric)

### Supporting KPIs

* Landing Page Visit Rate
* Trial Start Rate
* Paid Conversion Rate
* Revenue Per User
* Engagement Score

### Guardrail Metrics

* Refund Rate
* Support Ticket Rate
* Average Days to Convert
* Revenue Quality

The KPI tree illustrates how improvements in onboarding should drive activation, which in turn improves conversions and revenue while ensuring customer experience metrics remain healthy.

---

# 5. Experiment Analysis Approach

The analysis followed these steps:

1. Data quality validation

   * Missing values check
   * Duplicate user check
   * Binary value validation
   * Revenue outlier review

2. Experiment balance validation

   * Control vs Treatment counts
   * Region distribution
   * Device distribution
   * Traffic source distribution
   * Plan type distribution

3. KPI comparison

   * Conversion funnel metrics
   * Revenue metrics
   * Engagement metrics

4. Hypothesis testing

   * One-tailed proportion Z-test
   * Significance level: 5%

5. Guardrail evaluation

   * Refund Rate
   * Support Ticket Rate
   * Days to Convert
   * Engagement Score
   * Revenue Per User

---

# 6. Hypothesis Test Summary

### Null Hypothesis (H0)

The new onboarding experience does not improve Activation Rate.

H0: Treatment Activation Rate ≤ Control Activation Rate

### Alternative Hypothesis (H1)

The new onboarding experience improves Activation Rate.

H1: Treatment Activation Rate > Control Activation Rate

### Test Type

One-tailed proportion Z-test

### Significance Level

α = 0.05

### Test Results

| Metric         | Value  |
| -------------- | ------ |
| Control Rate   | 15.58% |
| Treatment Rate | 21.26% |
| Z-Score        | 2.74   |
| P-Value        | 0.003  |

### Decision

Reject the Null Hypothesis.

The Treatment group achieved a statistically significant improvement in Activation Rate.

---

# 7. Guardrail Metrics Considered

| Metric               | Control | Treatment | Assessment      |
| -------------------- | ------- | --------- | --------------- |
| Refund Rate          | 0.00%   | 0.42%     | Low Risk        |
| Support Ticket Rate  | 14.72%  | 24.76%    | Moderate Risk   |
| Avg Days to Convert  | 8.86    | 6.40      | Positive Impact |
| Avg Engagement Score | 57.03   | 62.93     | Positive Impact |
| Avg Revenue Per User | 51.75   | 53.88     | Positive Impact |

### Guardrail Conclusion

The experiment improved activation, engagement, revenue per user, and conversion speed. The primary concern is the increase in support ticket rate, which should be monitored after rollout.

---

# 8. Final Recommendation

## Recommendation: Launch

The Treatment experience should be launched to all users while monitoring support ticket volume.

Supporting evidence:

* Activation Rate increased significantly.
* Paid Conversion Rate improved.
* Revenue Per User increased.
* Engagement Score increased.
* Conversion time decreased.
* Refund Rate remained low.
* Statistical test confirmed significance (p = 0.003).

---

# 9. Assumptions and Limitations

### Assumptions

* Users were randomly assigned to Control and Treatment groups.
* Experiment data accurately reflects user behavior.
* Activation Rate is an appropriate North Star metric.

### Limitations

* Experiment duration may not fully capture long-term retention effects.
* Revenue quality should continue to be monitored after rollout.
* Increased support ticket volume suggests onboarding friction may still exist.
* Results may vary for future user cohorts.

---

# # 10. Screenshots Included

1. KPI Tree Screenshot
   - screenshots/kpi_tree_preview.png

2. Experiment Summary Metrics
   - screenshots/summary_metrics.png

3. Hypothesis Test Output
   - screenshots/hypothesis_test_output.png

---

# Conclusion

The new onboarding experience produced a statistically significant improvement in Activation Rate and generated positive downstream business outcomes. Although support ticket volume increased, overall business impact remains favorable. Based on the results, the Treatment experience is recommended for rollout with continued monitoring of customer support metrics.
