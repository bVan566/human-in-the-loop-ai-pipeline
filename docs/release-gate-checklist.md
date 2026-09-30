# Release Gate Checklist

A release gate should be short enough to use and specific enough to prevent optimistic assumptions.

## Pre-Release

- [ ] Artifact matches the approved scope.
- [ ] Required QA checks passed.
- [ ] Known exceptions are documented.
- [ ] Human approval is recorded when required.
- [ ] Release destination and version are correct.
- [ ] External action is within authorized scope.

## Post-Submission

- [ ] Submission result is recorded.
- [ ] "Submitted" is not treated as "live" unless the external system defines it that way.
- [ ] Processing or waiting state has an owner or monitoring rule.
- [ ] Failure routes to a defined repair path.

## Terminal Verification

- [ ] Authoritative terminal status is observed.
- [ ] Internal operational state is reconciled.
- [ ] Duplicate release is prevented.
- [ ] Downstream processes receive the correct terminal signal.
- [ ] The item is closed or intentionally transitions to another lifecycle.

## Escalate When

- requirements materially change;
- QA and production disagree on an unresolved release blocker;
- the external platform returns an unknown or unsafe state;
- authorization is missing;
- repeated failure suggests a systemic defect rather than an artifact defect; or
- the requested action creates a new commitment outside established scope.
