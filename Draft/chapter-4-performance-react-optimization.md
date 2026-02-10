# Chapter 4 --- Performance & React Optimization

In the previous chapter, we focused on writing clean and maintainable
code.

Now we focus on something users care about the most:

👉 **Speed**

Users do not see your code quality.\
Users do not know your architecture.

They only feel one thing:

-   Is the app fast or slow?

If the app is slow → users leave\
If the app is fast → users stay

So performance is directly connected to: - User experience - SEO
ranking - Conversion rate - Revenue - Customer trust

------------------------------------------------------------------------

# 📌 1. What is Frontend Performance?

Frontend performance means:

-   Pages load quickly
-   Buttons respond instantly
-   UI feels smooth
-   No lag or freezing
-   No layout jumping

Simple rule:

> Fast apps feel professional. Slow apps feel broken.

------------------------------------------------------------------------

# 📌 2. Why React Apps Become Slow

Common reasons:

-   Large bundle size
-   Too many re-renders
-   Heavy images
-   Blocking JavaScript
-   Unoptimized API calls
-   No lazy loading
-   Poor state management

Good news:

👉 Most performance issues are easy to fix with best practices.

------------------------------------------------------------------------

# 📌 3. Core Web Vitals (Most Important KPIs)

Google defined **Core Web Vitals** to measure real user experience.

These are industry-standard performance KPIs.

------------------------------------------------------------------------

## ✅ Largest Contentful Paint (LCP)

### What it means

Time to load the main visible content

### Simple explanation

How long until the page looks ready

### Target

  Status              Time
  ------------------- ---------
  Good                \< 2.5s
  Needs Improvement   2.5--4s
  Poor                \> 4s

👉 Target: **\< 2.5 seconds**

### How to improve

-   Reduce bundle size
-   Optimize images
-   Use CDN
-   Lazy load content

------------------------------------------------------------------------

## ✅ Interaction to Next Paint (INP/FID)

### What it means

How fast the app responds to user interaction

### Simple explanation

When user clicks → how fast does it react?

### Target

  Status   Time
  -------- ---------------
  Good     \< 100--200ms
  Poor     \> 300ms

👉 Target: **\< 100ms**

### How to improve

-   Avoid heavy JS on main thread
-   Split code
-   Use memoization
-   Optimize re-renders

------------------------------------------------------------------------

## ✅ Cumulative Layout Shift (CLS)

### What it means

Unexpected layout movement

### Simple explanation

Content jumping while loading

### Target

  Status   Score
  -------- ---------
  Good     \< 0.1
  Poor     \> 0.25

👉 Target: **\< 0.1**

### How to improve

-   Set image sizes
-   Avoid dynamic layout changes
-   Use skeleton loaders

------------------------------------------------------------------------

# 📌 4. Bundle Size Metrics

JavaScript size is the biggest performance factor.

Bigger JS = slower loading

------------------------------------------------------------------------

## KPIs

  Metric             Target
  ------------------ ----------------------
  Initial Bundle     \< 200KB (gzipped)
  Total JS           \< 500KB
  Lazy Loaded Code   70%+
  Trend              Stable or decreasing

------------------------------------------------------------------------

## Why it matters

Large bundles cause: - Slow mobile performance - Higher data usage -
Poor SEO - Higher bounce rate

------------------------------------------------------------------------

# 📌 5. Lighthouse Scores

Lighthouse is a free performance tool by Google.

It gives easy scores.

------------------------------------------------------------------------

## Targets

  Metric           Target
  ---------------- --------
  Performance      90+
  Accessibility    95+
  Best Practices   95+
  SEO              90+

------------------------------------------------------------------------

## Why useful

Easy to understand\
Great for juniors\
Quick feedback after changes

------------------------------------------------------------------------

# 📌 6. React-Specific Optimization KPIs

React has special performance patterns.

------------------------------------------------------------------------

## ✅ Re-render Efficiency

### What

Avoid unnecessary component re-renders

### Why

Too many renders slow UI

### How

-   React.memo
-   useMemo
-   useCallback
-   Proper state structure

------------------------------------------------------------------------

## ✅ Component Size

### Target

-   \< 300 lines per component
-   Single responsibility

### Why

Small components render faster and are easier to maintain

------------------------------------------------------------------------

## ✅ Lazy Loading

### Target

Load pages/components only when needed

### Tools

-   React.lazy
-   Suspense
-   Dynamic import()

### Why

Faster initial load

------------------------------------------------------------------------

## ✅ Image Optimization

### Target

-   Compressed images
-   WebP/AVIF format
-   Lazy loading

### Why

Images are usually 50--70% of page weight

------------------------------------------------------------------------

# 📌 7. How to Measure Performance

Use these tools:

-   Lighthouse
-   Chrome DevTools
-   Web Vitals extension
-   Vercel Analytics
-   Google PageSpeed
-   WebPageTest

Always measure before and after changes.

------------------------------------------------------------------------

# 📌 8. How Junior Developers Can Improve Performance

Simple daily habits:

-   Keep components small
-   Avoid heavy libraries
-   Lazy load routes
-   Use pagination
-   Optimize images
-   Remove unused code
-   Test Lighthouse before merge

Small habits make big differences.

------------------------------------------------------------------------

# 📌 9. Common Mistakes

### ❌ Importing large libraries for small tasks

Use lightweight alternatives

### ❌ Rendering huge lists

Use virtualization

### ❌ Not memoizing expensive components

Causes re-renders

### ❌ Loading everything at once

Use lazy loading

### ❌ Ignoring mobile performance

Always test on slow network

------------------------------------------------------------------------

# 📌 10. Summary

Performance helps us:

-   Keep users happy
-   Improve SEO
-   Reduce bounce rate
-   Increase conversions
-   Make app feel premium

Golden rules:

👉 Load less\
👉 Render less\
👉 Block less\
👉 Measure always

Next chapter we will cover **Reliability & Stability**, where we ensure
the app runs smoothly without crashes.

------------------------------------------------------------------------

# 📚 References

-   https://web.dev/vitals/
-   https://developer.chrome.com/docs/lighthouse/
-   https://react.dev/learn/optimizing-performance
-   https://pagespeed.web.dev/
-   https://webpagetest.org/
