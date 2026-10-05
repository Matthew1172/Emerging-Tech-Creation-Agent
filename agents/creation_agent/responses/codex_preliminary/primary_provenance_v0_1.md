# Preliminary primary-run provenance

- Producer: independent Codex subagent `/root/primary_run`, using the complete `work/creation_agent_primary_prompt.txt` packet; model-produced analytical JSON, not a canned fixture.
- Analysis/access date: 2026-10-05.
- No ChatGPT UI run was performed. This is preliminary Codex evidence, not the requested external ChatGPT execution record.
- No specialist instructions or frozen core were edited. No git operations or banking actions were performed. Banking controls were not verified.
- Browsed original sources live: Anthropic launch announcement (2024-11-25), MCP architecture pinned to 2026-07-28, JSON-RPC 2.0 specification (origin 2010-03-26; update 2013-01-04), Fielding dissertation chapter 5 (2000), and Toolformer research abstract (initial submission 2023-02-09). URLs are recorded in the response’s evidence entries.
- Important verification: the pinned MCP architecture explicitly describes stateless per-request version/capability metadata and `server/discover`. Do not silently replace this with older initialization/session descriptions. This run checked documentation, not running implementations or compatibility.
- Validation: `python3 tools/validate_response.py agents/creation_agent/responses/codex_preliminary/primary_response_v0_1.json` returned `VALIDATION PASSED`. This checks the existing basic structural contract only, not factual or analytical quality.

## Observed analytical weaknesses, preserved without revision

- Scientific/economic/organizational/market forces are unevenly substantiated. Toolformer supplies a scientific precursor, but the organizational and market explanations remain plausible inferences without independently measured causal evidence.
- The REST comparison includes all requested broad criteria but compresses interoperability and implementation burden into inference; it has no empirical REST adoption or multi-host MCP interoperability evidence.
- The source base is small and architecture-heavy. The exact-specification forecast is deliberately weak and does not incorporate current ecosystem governance or independently reported enterprise outcomes.
- The packet’s cross-case testing requirement is not completed by this primary-only file; a separate contrast run must test historical invariance and contextual change. The final abstention entry acknowledges that scope limit.
