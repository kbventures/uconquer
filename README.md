<p align="center">
  <img src="images/logo.png" width="220" alt="UConquer logo" />
</p>

<h1 align="center">UConquer</h1>

<p align="center">
  Proposal workflow app for freelancers: finds matching jobs, writes drafts, answers client questions, shows which skills the market wants, and tracks which proposals win.
</p>

<p align="center">
  <a href="https://kenb.netlify.app/projects/proposal-intelligence-workspace"><img src="https://img.shields.io/static/v1?label=|&message=CASE%20STUDY&color=23555f&style=plastic" alt="Case study" /></a>
  <img src="https://img.shields.io/static/v1?label=|&message=WALKTHROUGH%20ON%20REQUEST&color=cdf998&style=plastic" alt="Walkthrough on request" />
</p>

> **Production source code is proprietary and maintained in a private repository.**
> This repository is a public showcase only.

## What it does

UConquer helps freelancers send better proposals, faster, on a job marketplace.

A Chrome extension watches saved job searches. When a matching job appears, the app builds a draft from the freelancer's own template and sends it by email or Telegram. The freelancer reviews, edits, and sends.

Every sent proposal is logged. Replies, calls, and wins are tracked, so the freelancer can see which kinds of jobs and proposals actually work.

## Key features

- **Job alerts that check themselves:** the extension checks up to 3 saved searches during working hours. If checks stop, the freelancer is told.
- **Drafts the app builds, not the AI:** each letter is built from the freelancer's template. AI only fills the job-specific blanks. If the AI provider fails, a second one takes over; if both fail, the template is returned so no work is lost.
- **Saved answers for client questions:** questions from job posts are pulled out and grouped. Each answer is either pasted word for word or fitted to each job from the freelancer's own fact sheet.
- **Templates and A/B tests:** three ready-made templates plus up to two custom ones. Two templates can take turns on new drafts, with results on the Metrics page.
- **Proposal stats:** reply, interview, and win rates, from jobs clicked through to revenue per deal, with funnel, origin, and workday charts.
- **Skills in demand:** every skill on the jobs found, ranked by the freelancer's gaps or by best pay for least competition.
- **Market plans:** AI sorts up to 800 recent jobs into categories. The app counts jobs, pay, and missing skills, and the AI writes a plan from those counts. Numbers on the page come from the counts, never from the AI.
- **Billing and accounts:** Stripe plans with a free trial, email preferences, and account deletion.

## Tech stack

**Next.js · React · TypeScript · PostgreSQL · Neon · Clerk · OpenAI · Claude · Stripe · Docker · Playwright**

Plus a Chrome extension (Manifest V3) for job capture.

## My contributions

I designed and built UConquer end to end:

- Product design and UX
- Full-stack app: 29 modules, 117 versioned database migrations, account-scoped data from day one
- Chrome extension for job alerts and sent-proposal logging
- AI drafting pipeline with provider fallback and cost control
- Testing: more than 1,200 unit tests, plus route, database, API, and browser tests
- Code review and architecture review on every change, and a full codebase review each week ([how I review AI-written code](https://kenb.netlify.app/blog/how-i-review-ai-written-code))

## Contact

Want a quick 5-minute walkthrough? Reach me through my [GitHub profile](https://github.com/kbventures).
