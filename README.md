# Post-Call Automation Opportunity Mapper (n8n)

I built this after noticing a pattern.

Most of the hard work in automation doesn’t happen during the build.
It happens *after* the conversation — when someone has to turn messy notes
into a clear plan.

That step is repetitive, subjective, and surprisingly draining.

So instead of doing it manually every time, I automated the thinking.

---

## The problem this solves

After a discovery or consulting call, teams usually end up with:
- call recordings
- rough summaries
- half-formed ideas
- and a vague sense of “we should automate something here”

What’s missing is structure.

This system exists to turn post-call chaos into a clear,
prioritized automation plan — consistently.

---

## What this system does

At a high level:

Post-call input → structured analysis → automation plan + next steps

In practice:

1. A team member sends either:
   - a call summary
   - a transcript
   - or an audio recording
   into Telegram

2. The system:
   - transcribes audio if needed
   - extracts operational context
   - identifies bottlenecks
   - maps them to automation categories

3. It returns:
   - an Automation Opportunity Brief
   - plus recommended next steps and sequencing logic

No dashboards.
No templates.
Just clarity.

---

## Why Telegram

Telegram removes friction.

It’s fast, familiar, and already used for internal workflows.
The goal isn’t to introduce a new tool —
it’s to fit into how teams already work.

---

## What this demonstrates

This isn’t a client-facing product.

It’s a thinking tool.

It shows how I approach automation beyond wiring nodes:
- encoding judgment
- standardizing decisions
- and reducing cognitive load for teams doing complex work

Technically, it demonstrates:
- voice + text ingestion
- AI-driven structure extraction
- decision logic and prioritization
- clean internal tooling with n8n

---

## How it works (high-level)

1. Telegram receives text or audio  
2. Audio is transcribed if needed  
3. AI extracts structure and pain points  
4. AI applies automation prioritization logic  
5. A clean brief + next steps are sent back to Telegram  

The system doesn’t replace expertise.
It supports it.
