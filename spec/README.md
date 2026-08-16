# Normative documents

The specification is one core document plus one document per role
interface:

| Document | Defines | Status |
|---|---|---|
| `core.md` | Exchange semantics: task lifecycle, exactly-once claims, leases, streaming, cancellation, multi-phase tasks | not started |
| `provider.md` | Provider/Worker interface: capability advertisement, grant requests, metric publication, result streaming, drain | not started |
| `gateway.md` | Gateway interface: task submission, metadata, result relay ordering | not started |
| `policy.md` | Policy interface: constraints, objectives, fail-closed semantics, priority resolution | not started |
| `telemetry.md` | Usage and decision records | not started |
| `bindings/http.md` | Default transport binding: HTTP + JSON with SSE streaming | not started |
| `bindings/grpc.md` | Optional transport binding: gRPC | not started |

Requirement levels (MUST/SHOULD/MAY) follow
[RFC 2119](https://datatracker.ietf.org/doc/html/rfc2119) /
[RFC 8174](https://datatracker.ietf.org/doc/html/rfc8174).
