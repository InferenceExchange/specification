# Schemas

The message schemas for the IXP envelope: tasks, capability
advertisements, grants, leases, result chunks, and usage records.

- Schemas are defined in proto3 and use its
  [canonical JSON mapping](https://protobuf.dev/programming-guides/json/):
  the default wire format is JSON; proto3 serves as the IDL and
  enables mechanical compatibility gating.
- This directory is the **single source of truth**: every
  `ixp-<language>` library generates its types from here. Types are
  never hand-written per language.
- The client-facing payload (OpenAI-compatible) is carried as an
  opaque document and is deliberately **not** described here.
