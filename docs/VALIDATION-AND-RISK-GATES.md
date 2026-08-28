# Validation and Risk Gates

## Validation loop

Every meaningful change is checked against an explicit expectation:

```text
requirement
→ expected result
→ implementation
→ observed result
→ evidence review
→ accept, revise, or stop
```

The evidence can be a deterministic test, a fixed fixture, a structured
comparison, a log, a screenshot, or a human-reviewed artifact. A model's
confidence is not a test result.

## Risk gates

| Gate | Question | Required outcome |
| --- | --- | --- |
| Scope | Is this change inside the approved objective? | Continue only if bounded |
| Identity | Is the owner and reporting destination clear? | No anonymous handoff |
| Integration | Are dependencies sequenced and observable? | Isolate one failing layer |
| Validation | Do expected and actual behavior match? | Evidence or a deliberate stop |
| Privacy | Does the artifact expose protected information? | Remove or keep private |
| Consequence | Could the next action create material risk? | Human review required |
| Release | Is the result documented for the next owner? | Reusable handoff before close |

## Agent reporting

Agent work is useful only when another person can inspect what happened. A
handoff records the question, changed surface, evidence, limitations, and
next owner. If a requirement changes, the change is recorded rather than
silently substituted.

## Fail-closed behavior

When evidence is missing, a dependency is unresolved, or a result differs from
expectation, the system stops at review. It does not infer success from a
partial result. The safe states are:

- revise the implementation;
- request more evidence;
- escalate to the accountable human;
- defer the action.

## Public-safe boundary

This document intentionally uses generic examples. It does not publish private
thresholds, strategy logic, financial data, credentials, live operations,
collaborator identities, or private repository architecture. It also does not
claim that this method creates subject-matter authority in regulated or
safety-critical domains.
