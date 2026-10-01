# AdaptIQ — Personalised AI Tutor for Learning AI

Built for **Build Fast with AI / HACK 26** — Problem Statement **PS-03: Personalised AI Tutor for Learning AI**.

## What it does
AdaptIQ is an adaptive AI tutor. A learner takes a short diagnostic quiz, AdaptIQ builds a live
**skill map** of what they already know, and then:

- answers questions in a chat tutor pitched to their actual level (deeper on topics they
  know, first-principles + analogy on topics they don't),
- generates fresh practice questions targeted at their weakest topic on demand,
- shows the skill map itself, so progress is visible topic-by-topic instead of hidden
  behind "videos watched."

## Why we built it
Self-paced AI/ML learners get one fixed course path with no one to ask in the moment.
Doubts sit unanswered for days and quizzes are graded only after the fact, so gaps in
fundamentals surface weeks after they formed. AdaptIQ diagnoses first, then teaches to the
exact gap.

## Live demo
**[Try it here](https://claude.ai/artifact/M3C84K4K5RrDz7WLME79B7)**

## Tech
- Single-page app: plain HTML, CSS, and JavaScript — no build step.
- AI tutoring, explanations, and practice-question generation are powered by an LLM
  (Claude), called live from the browser with the learner's current skill map sent as
  context on every request — so every answer is actually personalised, not scripted.

## Running locally
This is a static page (`index.html`). Open it directly in a browser, or serve it:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

> Note: the AI tutoring and practice-question features call a sampling capability that is
> only available when the page is opened inside its hosted Claude artifact environment
> (see Live demo link above). Opened as a plain static file, the quiz and skill map still
> work; the chat will prompt that live tutoring needs the hosted environment.

## Team
**raushankumar.29ht** — Raushan Kumar · Gopal Kumar · Rishav Jha
