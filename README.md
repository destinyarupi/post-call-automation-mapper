# Post-Call Automation Opportunity Mapper (n8n)

This is a small internal tool built to support the *thinking* that happens
after discovery and consulting calls.

Most automation work doesn’t start with nodes or code.
It starts with turning messy conversations into clear, defensible decisions.

This system exists to make that step faster and more consistent.

---

## The problem it addresses

After a discovery call, teams usually have:
- a call recording or transcript
- rough notes or summaries
- a mental list of “things we could automate”

What’s missing is structure.

Turning that information into:
- a clear automation opportunity map
- a logical starting point
- and a phased implementation plan

…is valuable work, but it’s also repetitive and mentally expensive.

This tool supports that process.

---

## What this system does

At a high level:

Post-call input → structured analysis → automation brief + next steps

In practice:

1. A team member sends one of the following into Telegram:
   - a call summary
   - a transcript file
   - or an audio recording

2. The system:
   - transcribes audio if needed
   - extracts operational context
   - identifies bottlenecks
   - maps them to automation opportunities

3. It returns:
   - a structured Automation Opportunity Brief
   - plus recommended next steps and sequencing logic

This is intended for **internal use**, not clients.

---

## Why Telegram

Telegram keeps the workflow lightweight.

No dashboards.
No new interfaces.
Just a familiar place to drop post-call inputs and receive clarity.

---

## What this demonstrates

This system isn’t about automation for automation’s sake.

It demonstrates:
- how to encode consulting judgment
- how to standardize decision-making
- how to reduce post-call cognitive load
- and how to support delivery teams without replacing them

Technically, it shows:
- multi-input handling (text, file, audio)
- structured AI reasoning
- enforced output schemas
- clean internal tooling built with n8n

---

## How it works (high-level)

1. Telegram receives a message (text, file, or audio)
2. Audio is transcribed if necessary
3. A single AI agent analyzes the input
4. The agent outputs a structured automation brief
5. The result is formatted and sent back to Telegram

---

## Optional: Test the bot

The Telegram bot used for this workflow is live and can be tested
with your own call summaries, transcripts, or audio recordings.

This is an internal utility, not a client-facing tool.

👉 **Bot link:** [Post Call Mapper](https://t.me/post_call_mapper_bot)
