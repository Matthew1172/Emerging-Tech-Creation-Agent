# Lab 2 Emerging Technology Creation Agent

Version: 0.1-lab2. Status: specialized and ready for ChatGPT runs; no runtime results yet.

The agent examines MCP's creation and uses REST's architectural history as a bounded comparison. It does not implement an MCP server or connect to real banking systems.

- Primary: hypothetical conservative bank, read-only branch assistance.
- Contrast 1: same bank and technology, promotion enrollment and record writes.
- Contrast 2: same technology, small retailer with read-only catalog assistance.

Build each packet from the repository root:

```bash
python3 tools/build_prompt.py --agent agents/creation_agent --case agents/creation_agent/cases/primary.json
python3 tools/build_prompt.py --agent agents/creation_agent --case agents/creation_agent/cases/contrast_1.json
python3 tools/build_prompt.py --agent agents/creation_agent --case agents/creation_agent/cases/contrast_2.json
```

Paste the entire generated packet into ChatGPT, preferably in a separate conversation for each case, with browsing available for source verification. Save JSON-only outputs as responses/primary_response.json, responses/contrast_1_response.json, and optionally responses/contrast_2_response.json. Run the included validator on each output. The common validator is a basic structural check, not a factual assessment.

Record the actual stable/changed findings, preserve a weak output before revision, revise specialist instructions and metadata version, rebuild packets, and rerun the same cases. Finish the Agent Record with your own judgment. No API key is required. FROZEN CORE and shared tools are unchanged.
