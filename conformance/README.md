# Conformance

The executable conformance suite. Compliance with the specification
is defined by a passing run, not by prose interpretation.

- Tests are written against the normative statements in
  [../spec/](../spec/); a specification change that alters behavior
  must change the corresponding tests in the same pull request.
- The suite targets the default HTTP + JSON/SSE binding and runs
  against any implementation reachable at a URL, with no access to
  its internals.
