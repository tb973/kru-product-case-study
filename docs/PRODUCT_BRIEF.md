# KRU | Illustrative Product Brief

> A sanitized product management example informed by the project. It is not an assertion that this exact document was used as the original implementation specification.

## Opportunity

Users practicing Muay Thai alone often lack a simple sequence that links learning, practice, and improvement. A structured digital companion could reduce ambiguity at the start of a session.

## Objectives

1. Reduce friction between opening the product and beginning a session.
2. Provide useful guidance without pretending a camera or AI model is a human coach.
3. Make it easy to repeat a session and track completion.

## Primary user story

As a solo practitioner, I want a guided round with technique prompts and a clear timer so that I can practice without planning every exercise myself.

### Acceptance criteria

- A user can select an available practice type and start a timed session.
- Pause, resume, reset, and completion states are understandable and usable on mobile.
- Audio can be muted or disabled without blocking practice.
- If camera or AI functionality is unavailable, the interface clearly states what remains usable.
- No scoring or feedback claims unsupported precision.

## Secondary user story

As a learner, I want to submit a supported instructional video and receive a practice-oriented summary so that I can turn passive viewing into a concrete session.

### Acceptance criteria

- Invalid or unsupported links receive a helpful error.
- The workflow distinguishes submission, processing, result, and failure states.
- The system avoids claims about movements it cannot reliably identify.
- The user can review the summary before choosing to practice.

## Non-goals for the first release

- Medical or injury diagnosis.
- Certifying safe technique or guaranteeing fitness outcomes.
- Presenting estimated pose measurements as clinical-grade biomechanics.
- Automatically trusting unverifiable fighter data.

## Proposed metrics

Activation: users starting a first practice session.  
Engagement: completed sessions per weekly active learner.  
Quality: share of AI interactions rated useful; failure or retry rate.  
Economics: median third-party model cost per completed AI-assisted session.
