# KRU | AI Evaluation and Release Framework

> A public, non-technical example of the quality framework. It does not disclose proprietary evaluation prompts or any security-sensitive implementation details.

## Quality dimensions

| Dimension | Reviewer asks | Example failure |
| --- | --- | --- |
| Relevance | Does the response answer the user's training goal? | Generic advice disconnected from selected practice |
| Factual reliability | Are fighter or video observations supported? | Invented fighter details |
| Actionability | Can the user turn the answer into a reasonable drill? | Vague and non-executable plan |
| Uncertainty | Does the product disclose limits? | Claiming precision when the input is unclear |
| User safety | Are high-risk claims appropriately constrained? | Presenting an injury diagnosis as coaching |
| Performance | Is the experience responsive and recoverable? | Indefinite loading with no retry |
| Unit economics | Is model usage proportionate to delivered value? | Multiple avoidable calls for a single user action |

## Proposed launch gates

- Critical learner paths work on mobile and desktop.
- AI integration errors are recoverable without losing user context.
- Permission denial is handled for camera and audio.
- No published example reveals credentials or private user data.
- Test results, unresolved risks, and deployment configuration are reviewed separately.
- Release status is only marked complete when the actual hosted version is verified.

## Evidence policy

Recorded test counts, completion metrics, and live release status should be dated and linked to independent evidence before they are presented as final outcomes.
