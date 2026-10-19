# KRU · Product brief

Requirements and journeys below are reconstructed from the implemented application and its private product documentation, reviewed October 18, 2026.

## Problem and product hypothesis

Solo Muay Thai practice is fragmented across instructional videos, timers, and general advice. Connecting a short learning sequence to a playable session can reduce the planning required to begin practice. Whether this improves retention still requires learner validation.

## Core journeys and acceptance criteria

| User need | Journey | Acceptance criteria reflected in the product |
| :--- | :--- | :--- |
| Learn a fundamental | Choose a lesson, read the movement breakdown, continue to practice | The stages are explicit; stance and technique cues remain visible; the learner can return to the curriculum. |
| Work through a session | Select a program, start rounds, pause or resume, finish | Work and rest states are distinct; session controls are understandable; audio can be disabled. |
| Learn from a video | Enter a public YouTube link, choose a scan, process, review output | Invalid links are rejected; Shorts are recognized; processing has a failure path; identified moments and practice suggestions are structured. |
| Receive coaching | Ask a training question or request a combination | The request retains context; errors permit retry; the coach does not claim to have watched the user in text chat. |
| Train from a fighter’s style | Search, resolve identity, set training preferences, review a program | Fighter identity is checked; unsupported facts are left unknown; a fallback is labeled as an archetype rather than fighter analysis. |
| Use camera feedback | Choose supported tracking, grant permission, practice slowly | Permission and detection states are handled; feedback does not claim a complete technique assessment or medical accuracy. |

These criteria describe intended behavior and existing controls. Release verification is tracked separately in the [QA record](EVALUATION_AND_RELEASE.md).

## Prioritization rationale

| Priority | Product work | Why it comes first |
| :--- | :--- | :--- |
| Core training value | Fundamentals, guided rounds, session controls | A learner should be able to practice without waiting for advanced AI. |
| Trust and recovery | Verified fighter identity, honest fallbacks, valid output, clear errors | Incorrect certainty damages both the session and confidence in the product. |
| Reliable AI workflows | Coaching, video interpretation, provider limits, caching | Useful output must remain responsive and financially sustainable. |
| Progression depth | Longer programs and future progression features | Expand after the core experience and release gates are reliable. |

## Scope boundaries

The application supports educational solo practice. Injury diagnosis, training clearance, guaranteed fitness outcomes, and precise grading of an entire fighter style are outside the product promise. The roadmap does not treat those boundaries as unfinished features.

## Measures for future validation

First session completion, return to practice, video completion and retry rates, coaching usefulness, and cost per successful assisted session are appropriate next measurements. No user growth, retention improvement, or revenue result has been verified for this case study.
