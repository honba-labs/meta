# `meta` Agent Guidelines & Architecture Invariants

**Subsystem**: Meta (Cross-Repository Tooling & Release Management)
**Language**: Shell / Python
**Primary Responsibility**: Workspace-wide scripts, dependency graph verification, release tagging, and cross-repo synchronization.

---

## 1. Role & Architectural Hints
* `meta` manages cross-cutting workspace tooling:
  1. Multi-repo dependency synchronization.
  2. Workspace-wide cargo and python test runners.
  3. Release coordination and version bumping.

---

## 2. Guidelines
* Ensure all cross-repo scripts respect `.agents/` as the single canonical agent directory.
* Never introduce hard vendor dependencies.
