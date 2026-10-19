# KRU · Quality and release readiness

## Evidence reviewed

| Evidence | What it establishes |
| :--- | :--- |
| October 12, 2026 AI Product Manager resume | A reported 107-test release candidate and production safety review, with the website update still pending. |
| Private application source and existing tests | Implemented workflows and regression coverage for fighter research, fallback behavior, video parsing, motion, timing, voice, and account related logic. |
| Private training phase documentation | Completed Phase 1 session work, with Phase 2 progression and Phase 3 optional clip feedback separated as future work. |
| Hosted application review on October 18, 2026 | Visible home, lesson, and video entry screens captured for this portfolio. |

**107 tests is a historical release candidate figure.** It is not a fresh result from the current repository. No current full KRU suite or live paid provider benchmark was run for this portfolio review.

## QA coverage and release gates

| Area | Existing evidence | Remaining release check |
| :--- | :--- | :--- |
| Fighter personalization | Verification, evidence parsing, structured plans, fallback tests | Live identity lookup and generated session quality across supported inputs. |
| Video | URL parsing, structured response handling, Quick and Deep paths | Hosted provider access, completed analysis, timeout recovery, and save behavior. |
| Sessions | Timer and work/rest tests; lesson and pad interfaces | Mobile controls, completion, pause, resume, and audio on real devices. |
| Camera | Pose and motion logic with test coverage | Permission denial, uncertain detection, camera framing, and supported-device behavior. |
| Voice | Policy and fallback checks | Playback, muting, device speech support, and interruption behavior. |
| Accounts | Account and training state logic | Sign in, ownership of saved activity, and failure recovery in the hosted environment. |

Provider errors and passing local tests are reviewed separately from launch readiness. KRU remains **in development**.

## Development roadmap

| Stage | Scope | Status |
| :--- | :--- | :--- |
| Foundation | Lessons, guided rounds, camera practice, video and coach interfaces | Implemented; continued validation. |
| Phase 1 session upgrades | Style archetypes, training preferences, playable rounds, voice fallback, video discovery | Documented in private product materials and implemented paths. |
| Release hardening | Consistent provider models, hosted integration checks, real device media QA | Ongoing release work. |
| Phase 2 progression | Multiweek camps, scorecards, check-ins, challenges, and earned unlocks | Planned; not presented as shipped. |
| Phase 3 optional clip feedback | Explicit short uploads, educational feedback, retention and privacy controls | Planned; no automatic recording of live training. |

## Launch decision

A release should clear the critical learner journeys, output quality, provider access, user data controls, real device media checks, and rollback review. The existence of a deployed interface does not establish that the release candidate has completed those checks.
