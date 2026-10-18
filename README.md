# KRU | AI Coaching Product Case Study

**Domain:** Consumer fitness and sports technology  
**Focus:** AI Product Management, product discovery, iterative delivery, quality and release readiness  
**My role:** Independent product owner and AI-assisted development lead  
**Product status:** In active development; release candidate work has been documented, but a completed production release is not claimed.

## The problem

Solo Muay Thai practitioners can struggle to structure sessions, translate instructional video into safe practice, and obtain timely technique feedback without always having an in-person coach available.

## Product hypothesis

A guided training experience that connects fundamentals, timed practice, video-based learning, and contextual coaching can help users practice more consistently and with greater clarity.

**Target users:** Beginners learning the basics and intermediate solo practitioners looking for more structured practice.  
**Core job to be done:** “Help me know what to practice, how to practice, and what to improve next.”

## My product ownership

- Defined the initial product vision and mapped the progression from lesson to drill to round review.
- Prioritized camera-guided training, AI coaching, video breakdowns, fighter-inspired workouts, and account-based progress as distinct product workflows.
- Specified user inputs and guardrails for personalized workouts, including training experience and goals.
- Directed AI-assisted development iterations, reviewed API capabilities and limits, and defined acceptance testing scenarios.
- Balanced user experience with service reliability, operating cost, and staged release readiness.

## Experience design

| Product area | User value | Product consideration |
| --- | --- | --- |
| Guided fundamentals | Clear path for learning stance, strikes, and movement | Short sessions, readable cues, sensible progression |
| Camera-guided practice | Visual practice feedback in the training flow | Device support, camera permission, uncertain detections |
| Video-to-practice | Convert relevant instruction into an actionable practice plan | Video availability, interpretation accuracy, safe coaching language |
| AI coach | Ask questions and receive contextual training suggestions | Responses should not imply certainty where the model is unsure |
| Fighter-inspired plans | Explore styles and tailor a session | Verify fighter information rather than fabricate profiles |
| Training history | Help users resume and assess consistency | Distinguish saved activity from unverified performance claims |

## Key product decisions

**Start with a usable training loop.** A short progression from fundamentals to timed sessions makes the product valuable before every advanced feature is available.

**Separate AI outputs from verified facts.** Fighter details and instructional video interpretations require clear sourcing, confidence, or appropriate fallback behavior.

**Treat usage cost as a product constraint.** AI calls, caching, request limits, and alternative experience paths influence feature design and release order.

**Release incrementally.** Camera and audio features require real-device verification, not just a passing interface or a local browser test.

## Delivery and validation

Product work included requirement definition, iterative review with coding agents, API integration review, browser interactions, and release-candidate checks. Project records describe a **107-test release candidate**; this figure is historical project reporting rather than a new independent test run or proof of production deployment.

The release decision remains conditional on integration credentials, hosted environment checks, and real-device media behavior.

## Outcome and what is next

KRU is a substantive, continuing product build with implemented interactive learning and AI-related workflows. The immediate product objective is to validate a reliable end-to-end learner experience before expanding feature depth or monetization.

**Success measures to track, not claimed outcomes:** first-session completion, weekly practice retention, analysis completion rate, coaching helpfulness, per-session AI cost, and media workflow reliability.

## Supporting product artifacts

- [Illustrative product brief and acceptance criteria](docs/PRODUCT_BRIEF.md)
- [Decision log](docs/DECISION_LOG.md)
- [AI and release evaluation plan](docs/EVALUATION_AND_RELEASE.md)

## What this public case study does not contain

This repository includes **no application source code**, deployment secrets, internal prompts, production credentials, private user records, or proprietary training algorithms. Product screens can be added after checking that they do not expose private information.
