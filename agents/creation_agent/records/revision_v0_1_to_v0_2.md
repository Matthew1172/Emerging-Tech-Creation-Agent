# Observed weakness and revision

Runtime: preliminary independent Codex subagents, 2026-10-05. These are not ChatGPT UI executions.

Preserved weak output: responses/codex_preliminary/contrast_2_response_v0_1.json. Its contrary_evidence_or_limitations requests bank-specific architecture, permissions, eligibility rules and review controls; its abstention_or_more_information_needed again requests bank-specific evidence despite the active case being a retailer. This is an observed context-sensitivity failure even though structural validation passed.

Cause: v0.1 instructions required missing bank-specific facts for every case and stated banking constraints without explicit case gating. The retail case also contains residual banking wording in additional_context. We deliberately keep all cases unchanged for the retest so we test the instructions rather than removing the trigger.

Revision: v0.2 gates organization-specific requirements by the active intake fields, handles inconsistent residual context without importing irrelevant requirements, and asks retail-only runs for retail evidence. Additional improvements target dense management prose and the observed lack of original model-capability research in two initial outputs. No claim of a completed empirical account of REST market success is made.

Retest: rerun the same three case files; preserve v0.1 responses and configuration. Compare bank-specific requests in the retail output, stable historical findings, and appropriate banking read/write distinctions. Observed outcome: retail v0.2 no longer requests banking evidence; all six outputs pass structural validation. See preliminary_test_comparison.md for paired observations and residual limitations.
