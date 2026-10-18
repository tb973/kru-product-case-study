# KRU | Product Decision Log

> Sanitized, retrospective examples of product decisions. No internal implementation details or prompts are included.

| Decision | Alternatives considered | Rationale | Tradeoff |
| --- | --- | --- | --- |
| Prioritize basic guided lessons and timed rounds | Start with video AI analysis first | Makes the core learning journey usable without third-party processing | Less immediate technical novelty |
| Include camera and video features as separate workflows | Combine all analysis in a single screen | Different user permissions, input quality, failure states, and learning contexts | More screens to maintain |
| Include explicit uncertainty or fallback messaging | Always return a definitive coaching answer | Protects user trust when AI outputs or source data are unreliable | Some responses are less polished |
| Require real-device checks for audio and camera | Treat local desktop testing as sufficient | Browser permissions and hardware vary substantially | Slower release validation |
| Track AI service costs as a product metric | Optimize only for feature count | Supports scalable economics and sensible limits | Requires prioritizing efficiency |

## Example prioritization approach

Evaluate each candidate against user value, evidence, implementation complexity, model cost, reliability, and safety. Do not interpret a single score as a substitute for product judgment.

## Follow-up questions

- Which features actually improve completion and retention?
- Where do users abandon video processing?
- Which coaching outcomes need stronger confidence labeling?
- Can a usable no-AI practice mode preserve value when a provider is unavailable?
