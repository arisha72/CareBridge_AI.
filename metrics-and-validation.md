# Metrics and Validation Plan

All figures below are **proposed targets**, not achieved results or validated benchmarks.

## North-star outcome
Percentage of enrolled care recipients who successfully complete their intended medication routine over a defined period, based on user-reported events. This is an adherence proxy, not proof that medication was ingested.

## MVP metric tree

| Area | Metric | Definition |
|---|---|---|
| Activation | Setup completion rate | Users who complete profile and first schedule / users who start setup |
| Engagement | Weekly active care recipients | Care recipients with at least one meaningful weekly action |
| Reminder usefulness | Reminder acknowledgement rate | Reminders followed by a user status update within the chosen window |
| Routine visibility | Shared event coverage | Scheduled events with a recorded status / total scheduled events |
| Family value | Family dashboard weekly usage | Authorised supporters who view the dashboard in a week |
| Reliability | Notification delivery success | Successfully delivered notifications / attempted deliveries |
| Safety | OCR correction rate | Extracted fields edited by users / fields reviewed |
| Trust | Consent revocation and support rate | Track with qualitative feedback; interpret carefully |
| Satisfaction | Post-task satisfaction | Short usability rating after key tasks |

## Pilot plan
The original concept proposed a 20-family pilot. Treat this as an initial usability pilot, not a statistically powered clinical study.

1. Recruit a small, diverse set of older adults and family supporters.
2. Obtain informed consent and define exactly what data is shared.
3. Observe onboarding, schedule creation, reminder acknowledgement, and family-dashboard use.
4. Record notification failures and user confusion.
5. Conduct weekly interviews and collect task-level feedback.
6. Report actual results, sample size, dates, and limitations.

## Original proposal targets to test
- 85%+ medication routine completion / adherence proxy.
- 95% missed-event detection accuracy.
- Under 2 minutes average family alert time.
- 70% daily active usage among enrolled families.
- 4.5+ / 5 satisfaction.
- 80% of families reporting reduced worry.

Before using these targets publicly, define denominators, measurement windows, instrumentation, and baseline. In particular, “missed-dose detection accuracy” is not measurable unless the product has a reliable ground truth for whether a dose was actually taken.

## Experiment backlog
- Compare reminder presentation: simple text vs. voice prompt.
- Test large-button and simplified navigation variants.
- Test family dashboard labels for taken, skipped, and unconfirmed.
- Test consent comprehension with scenario-based tasks.
- Measure OCR correction burden on a varied set of prescription formats.
