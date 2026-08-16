# Inference Exchange Protocol (IXP) — Specification

**An open protocol for autonomous providers to advertise capabilities
and exchange LLM inference workloads across clouds, regions, and
organizations.**

> **Status: drafting.** Nothing in this repository is stable yet.
> Follow and join the discussion in the
> [organization Discussions](https://github.com/orgs/InferenceExchange/discussions).

## Layout

| Directory | Contents |
|---|---|
| [spec/](spec/) | The normative documents: core exchange semantics and the role interfaces |
| [schema/](schema/) | Message schemas — the single source of truth for all language libraries |
| [rfcs/](rfcs/) | Design proposals and their record |
| [conformance/](conformance/) | The executable conformance suite; compliance is a passing run |

## Design principles

- The specification defines **observable semantics**, not
  implementation substrates.
- The default transport binding is **HTTP + JSON with SSE streaming**;
  other transports are optional extensions.
- The client-facing payload is the OpenAI-compatible API, carried
  opaque and never transcoded: IXP is the envelope, not the prompt
  schema.
- Per-language libraries follow the `ixp-<language>` repository naming
  and generate their types from [schema/](schema/); types are never
  hand-written per language.

## Versioning

During drafting, revisions are date-based (`YYYY-MM-DD`). Semantic
versioning starts with the first stable release. Schema compatibility
is gated mechanically in CI.

## Contributing

Substantial changes start as an RFC — see [rfcs/](rfcs/). Everything
else follows the organization-wide
[contributing guide](https://github.com/InferenceExchange/.github/blob/main/CONTRIBUTING.md)
and [governance](https://github.com/InferenceExchange/.github/blob/main/GOVERNANCE.md).

## License

[Apache 2.0](LICENSE)
