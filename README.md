**Hi, I'm Irfan.** I build reliability tooling for LLM systems: schema gates that refuse bad
output, failure taxonomies that give bugs names, eval harnesses whose numbers you can recompute
yourself. By day that means agent pipelines that turn requirements into reviewed, tested
changes, with validation gates between every stage. The open-source work is the same discipline
with all the evidence published.

## Shipped

Everything in this section obeys one rule: it runs, and every number it claims can be
recomputed from evidence committed in the repo. A claim that cannot be recomputed is marketing.
The rule keeps the list short, and short is fine.

**[load-board-matcher](https://github.com/amirfandev/load-board-matcher)**
An LLM extraction pipeline behind a pydantic schema gate. Output that fails validation is
neither accepted nor fatal: the failure is classified into a named taxonomy and the model
retries with its errors in hand. 186 tests, CI on Python 3.11 and 3.12, MIT. The eval harness
runs an 8-case golden set with the raw model responses committed in the repo, so every
published figure can be recomputed from the data that produced it.

## On the bench

Three problems, same territory: catching context compaction that silently drops a safety
constraint or task invariant, putting a deterministic policy gate in front of agent tool calls,
and bringing this eval discipline to on-device models on Apple platforms. Nothing here gets a
name, a link, or a date until it ships and its claims hold. When one clears the bar, it moves
up. Until then it is a problem, not a promise.

## How I build

- **Runnable over described.** If you can't clone it and run it, it's a claim, not a tool.
- **Numbers carry their evidence.** An eval result without the raw data behind it is an
  anecdote with a decimal point.
- **Failures get names.** "Wrong" is not a category. "Unit confusion in numeric fields" is. A
  named failure class with a test attached can be counted, fixed, and watched for regressions.
- **One problem per repo.** Small tools compose. Platforms rot.

None of this is a new habit. Thirteen years of iOS and real-time media came first, including a
60fps camera app that passed 8 million downloads and the original Flashlight app at number one
in App Store Utilities. Then four years as tech lead on a healthcare EMR platform in Abu Dhabi,
where the systems carried e-prescriptions and I ran the internal HIPAA and ADHICS audits. Hard
gates stopped being a style preference somewhere in there.

If something breaks, or a number doesn't recompute, open an issue. That is the fastest way to
reach me. And if you are hitting agent failure modes that don't have names yet, I want to hear
about those too: [LinkedIn](https://www.linkedin.com/in/am-irfan).
