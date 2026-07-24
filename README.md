I work on the part of applied AI that decides whether a system can be trusted in production.
Structured output validation, golden-task evals, failure taxonomies, and the guardrails that
turn "the agent broke" into a named, testable class of bug.

### Building

**[load-board-matcher](https://github.com/amirfandev/load-board-matcher)** is an LLM extraction
pipeline behind a schema gate. It classifies every failure into a named kind and retries with
the errors, rather than crashing on bad output or accepting it. It ships with an eval harness
over a golden set of eight calls, and every published number can be recomputed from the raw
responses committed beside it.

### Before this

Thirteen years building production software, most of it mobile.

**Regulated healthcare, four years, Abu Dhabi.** Tech lead on an EMR platform: appointment
workflows, HL7, e-prescriptions, pharmacy integrations, in-app payments. Implemented the
ADHICS, HIPAA, ISO 27001 and GDPR workflows and ran the internal audits.

**Consumer iOS at scale.** A real-time 60fps camera app that passed 8 million downloads, a
video editing app that took Best of Show at Macworld, and the original Flashlight app at number
one in App Store Utilities.

Both of those turn out to be the same job as the current one. Decide what correct means, measure
it, and fail loudly when it is not. The difference now is that a model hands you a plausible
wrong answer instead of a crash, so nothing tells you to go looking.

am_irfan@outlook.com · [LinkedIn](https://www.linkedin.com/in/am-irfan)
