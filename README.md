# osstack-bridge-sandbox

Sandbox for the osstack ↔ Grok Bots bridge (osborn-studio/osstack ADR-006, plan phase 2).

- Rulesets from `osborn-studio/osstack/.github/rulesets` are applied here first.
- `scripts/bridge-probe-github.mjs` runs destructive probes (P-1 … P-12) only against this repository.
- The CI here is a stub: it reports the same five required check names as osstack's CI. A commit that contains a `PROBE_FAIL` file makes every check fail, so probes can test merges with a failing check.

Nothing here is production code. Do not store secrets or keys in this repository.
