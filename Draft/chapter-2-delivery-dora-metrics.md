# Chapter 2 --- Delivery & DORA Metrics

In this chapter, we focus on one simple question:

👉 **How quickly and safely can our React team ship changes to users?**

Shipping fast is good.\
Shipping safe is also important.

Great teams balance both.

This chapter explains **Delivery KPIs** and **DORA Metrics**, which are
globally accepted standards used by high‑performing engineering teams.

------------------------------------------------------------------------

# 📌 1. What are Delivery Metrics?

Delivery metrics measure:

-   How fast we release
-   How stable releases are
-   How often things break
-   How quickly we fix problems

If delivery is slow → users wait\
If delivery is risky → production bugs increase

So we need **speed + stability together**.

------------------------------------------------------------------------

# 📌 2. What are DORA Metrics?

DORA stands for:

**DevOps Research & Assessment**

Google and DevOps experts studied thousands of teams and found **4
metrics** that predict engineering success.

These 4 are called:

> ⭐ The Golden 4 Metrics

1.  Deployment Frequency
2.  Lead Time for Changes
3.  Change Failure Rate
4.  Mean Time to Recovery (MTTR)

If these improve → your team performance improves automatically.

------------------------------------------------------------------------

# 📌 3. Deployment Frequency

## What it means

How often we deploy code to production.

## Simple explanation

How many times users receive updates.

## Why it matters

More deployments mean: - Faster feature delivery - Faster bug fixes -
Smaller and safer releases

Big releases = risky\
Small frequent releases = safe

## How to measure

Number of production deployments per day/week.

## Target

  Level    Frequency
  -------- -------------------
  Elite    Multiple per day
  High     Daily
  Medium   Weekly
  Low      Monthly or slower

👉 Target: **Daily or multiple per week**

## Tools

-   GitHub Actions / GitLab CI
-   Vercel / Netlify logs
-   CI/CD dashboards

## Example

Bad: 1 release every month\
Good: 3--5 releases per week

------------------------------------------------------------------------

# 📌 4. Lead Time for Changes

## What it means

Time from code commit → production.

## Simple explanation

How long a feature waits before users see it.

## Why it matters

Long lead time means: - Slow reviews - Manual testing delays -
Deployment bottlenecks

Short lead time means: - Fast feedback - Happy users - Quick iteration

## How to measure

Commit timestamp → deployment timestamp

## Target

  Level    Time
  -------- ------------
  Elite    \< 1 day
  High     1--7 days
  Medium   1--4 weeks
  Low      \> 1 month

👉 Target: **Under 1 week (ideally 1--2 days)**

## Tools

-   Git logs
-   Jira cycle time reports
-   CI/CD timestamps

## Example

Bad: Feature takes 3 weeks to release\
Good: Feature released same or next day

------------------------------------------------------------------------

# 📌 5. Change Failure Rate

## What it means

Percentage of deployments that cause production issues.

## Simple explanation

How many releases break something.

## Why it matters

Frequent failures mean: - Poor testing - Risky changes - Unstable code

Stable releases build trust.

## How to measure

(Deployments with bugs or rollback ÷ total deployments) × 100

## Target

  Level    Failure Rate
  -------- --------------
  Elite    0--15%
  High     16--30%
  Medium   31--45%
  Low      \> 45%

👉 Target: **Below 15%**

## Tools

-   Incident tracking
-   Sentry
-   Rollback logs

## Example

Bad: 5 of 10 releases fail (50%)\
Good: 1 of 10 releases fail (10%)

------------------------------------------------------------------------

# 📌 6. Mean Time to Recovery (MTTR)

## What it means

How long it takes to fix production issues.

## Simple explanation

When something breaks, how fast do we fix it?

## Why it matters

Users don't care about bugs --- they care about downtime.

Faster recovery = better reliability.

## How to measure

Incident start → incident resolved

## Target

  Level    Recovery Time
  -------- ---------------
  Elite    \< 1 hour
  High     \< 1 day
  Medium   1--7 days
  Low      \> 1 week

👉 Target: **Less than 24 hours**

## Tools

-   Incident tools
-   Sentry alerts
-   Monitoring dashboards

## Example

Bad: Bug fixed in 4 days\
Good: Bug fixed in 2 hours

------------------------------------------------------------------------

# 📌 7. Additional Agile Delivery KPIs

Besides DORA, React teams also track:

------------------------------------------------------------------------

## Sprint Velocity

### What

Story points completed per sprint

### Why

Helps planning and prediction

### Target

Stable trend (not necessarily increasing)

------------------------------------------------------------------------

## Cycle Time

### What

Time from "In Progress" → "Done"

### Why

Shows workflow efficiency

### Target

Small tasks: 1--3 days

------------------------------------------------------------------------

## Commitment Reliability

### What

\% of planned work completed in sprint

### Why

Shows planning accuracy

### Target

85--95%

------------------------------------------------------------------------

# 📌 8. How Junior Developers Can Improve Delivery

Simple habits:

-   Keep PRs small
-   Write tests
-   Avoid big risky changes
-   Merge frequently
-   Automate everything
-   Fix bugs quickly
-   Don't wait for big releases

Small improvements daily → big results monthly

------------------------------------------------------------------------

# 📌 9. Common Mistakes

### ❌ Big releases once a month

Very risky

### ❌ Manual deployments

Slow and error-prone

### ❌ Large PRs (2000+ lines)

Hard to review

### ❌ Ignoring incidents

Leads to repeated failures

### ❌ Measuring individuals

Always measure team delivery

------------------------------------------------------------------------

# 📌 10. Summary

Delivery metrics help us:

-   Ship faster
-   Reduce risk
-   Fix issues quickly
-   Keep users happy

Golden rule:

👉 Deploy small\
👉 Deploy often\
👉 Recover fast

Next chapter will cover **Code Quality & Engineering Excellence**, where
we focus on writing clean and maintainable React code.

------------------------------------------------------------------------

# 📚 References

-   https://dora.dev/
-   https://cloud.google.com/devops
-   https://www.atlassian.com/devops/frameworks/dora-metrics
-   https://martinfowler.com/articles/continuousIntegration.html
