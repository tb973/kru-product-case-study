# KRU · AI and architectural decisions

This record summarizes decisions visible in the private application and its development history. It contains product level reasoning, not internal prompts or service configuration.

## Provider evaluation

| Service | Role in the product | Evaluation and tradeoff |
| :--- | :--- | :--- |
| Groq | Conversational coaching and combination suggestions | A text focused path for short, contextual answers. Provider availability, request limits, output quality, and response length constrain the experience. |
| Gemini | Video interpretation, fighter related analysis, and structured training generation | Multimodal and structured output capabilities fit these tasks. Longer processing, quota pressure, and validation requirements are the tradeoff. |
| YouTube APIs | Fighter video discovery and public video metadata | Confirms availability, duration, and embed suitability. Metadata is not movement analysis and does not establish that a video is accurate instruction. |
| On device pose tracking | Camera based fundamentals feedback | Keeps live pose processing local and avoids a model request for each frame. Camera position and limited detection quality constrain the feedback. |

The code supports alternative coaching integrations, but selecting a configured provider is distinct from automatic failover after a failed request. The portfolio does not promise universal provider switching.

## Model selection and reliability

Models are selected by task rather than using a single model for every feature. Text coaching needs useful conversational replies; video work needs multimodal interpretation; generated programs need structured, validated output.

Development records include model availability changes and migration work. The next release needs a consistent, available model set and live checks of the affected journeys. Model names in development code are not proof that a hosted integration is working.

| Decision | Benefit | Cost or limitation |
| :--- | :--- | :--- |
| Quick and Deep video scan choices | Match processing effort to the learner’s immediate need | Deeper work may wait longer and consume more provider capacity. |
| Cache reusable analyses and discovery results | Avoid repeat work and reduce external requests | Cached information needs refresh and validation. |
| Bound requests, wait time, and output | Control cost exposure and make failures recoverable | Some work must be shortened or retried. |
| Validate structured output before use | Prevent malformed plans from becoming playable sessions | A fluent response can still be rejected. |
| Verify fighter identity before personalization | Reduce invented biographies and unsupported technique claims | Ambiguous or weak evidence can limit personalization. |
| Offer an explicitly labeled archetype fallback | Preserve useful practice during a failed lookup | The fallback must not be presented as analysis of a specific fighter. |

There is no verified cost per session or paid tier economics in the reviewed evidence. The implemented controls demonstrate cost awareness; a measured provider scorecard remains future work.

## Architectural boundaries

The interface handles learning and session interaction. Server side services handle external AI and video requests. Pose tracking runs in the browser, while account features handle saved training state separately.

This separation supports three product goals: keep provider credentials away from the interface, preserve a training experience when an external service fails, and distinguish saved user activity from public training material.

## Open evaluation questions

1. Which provider and model combination gives the most useful answer for each supported task?
2. Where do users leave video processing, and which errors should offer a shorter scan?
3. Does the archetype fallback remain clear and useful to learners?
4. What is the cost per completed coaching or video task after retries and cache use?

These are evaluation questions, not completed benchmarks.
