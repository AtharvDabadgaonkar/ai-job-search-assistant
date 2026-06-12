# AI-Powered Job Search Assistant (B2C)

## What this is

Jobseer is a concept product that takes the most painful part of job hunting - tailoring every application - and makes the AI do it. You tell the assistant what you want, it matches roles, tailors your resume per job, and surfaces a ready-to-apply queue.

This repo is a fully interactive case study: a working product slice embedded in the PM story that produced it. No backend, no build step — just open index.html.


## Key results

Metric
Result
Application click-through lift+28% (A/B tested)Scope0 → 1, roadmap through tested MVPAnalysis methodSQL funnel analysis


## What the demo shows

## AI assistant (left panel)
A clickable chat interface that walks through the core flow — surface PM roles, tailor a resume, explain job recommendations. Reflects the actual UX from usability testing.

## Live application funnel (right panel)
Animates as the assistant works: Roles matched → Viewed → Tailored & ready → Applied. Shows the funnel the team measured and optimized.

## A/B test breakdown
The experiment that moved the numbers. Variant A used a generic "Submit application" CTA. Variant B led with "Apply with tailored resume →" and pre-surfaced the resume tailoring step. Variant B won at statistical significance, confirmed by SQL analysis of the full funnel.

## Process section
Four-step breakdown of the PM lifecycle: Discover → Define → Design → Measure, with the artifacts and tools at each stage.


PM artifacts

Stage DeliverableTool - Discover User interviews, journey mapping, Research Define Roadmap, PRDs, user stories Jira, Prototypes, clickable usability tests, Figma , Measure , A/B test, funnel analysis , SQL, A/B testing


## The experiment

- Hypothesis: The generic "Submit application" CTA and buried tailoring step were the primary friction point in the apply funnel, not role-match quality.

- Setup: Split traffic 50/50 between two variants of the apply screen. Ran until statistical significance. Read the full funnel in SQL.

 - Result: Variant B (action-oriented CTA + pre-tailored resume) produced +28% click-through and a meaningfully higher completed-apply rate.

 - Learning: Users weren't dropping because they didn't want the job — they were dropping because tailoring felt like extra work. Moving that step upstream,      and naming it in the CTA, was the fix.

## Tech
Single self-contained HTML file. No framework, no build step, no dependencies.
- Layout and animation: vanilla CSS (custom properties, grid, keyframes)
- Interactivity: vanilla JS (chat flow, funnel animation, A/B stat simulation)
- Typography: Google Fonts (Fraunces, Inter, JetBrains Mono)

## Author
Atharv Dabadgaonkar
