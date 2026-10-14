# Validation

Validation date: 2026-10-14. This is an initial instruction-only release, not a guarantee of 100-turn reliability or marketing effectiveness.

## Structural checks

- Required `SKILL.md` entry point, skill name, description and supported YAML fields: passed with Ruby's YAML parser.
- UI YAML, short-description length and explicit default invocation: passed.
- Linked runtime references: present and readable.
- Generic runtime guidance: no hardcoded ONYX name or business-specific media policy.
- Preserved ONYX example: byte-identical to the original prompt file.
- No private interview ledger or real interview answers included.

The official `quick_validate.py` was attempted with both the system and bundled Python runtimes. Both could not import PyYAML. Equivalent parser and structural checks were completed with the available Ruby YAML parser instead. This package itself has no runtime dependency on Python, Ruby or YAML libraries; the host loads its Markdown instructions.

## Behavioral validation

Three independent Codex agent passes executed 13 distinct fictional fixtures and 3 repeated executions after clarification of the instructions. The maintainer inspected the raw outputs, rather than relying solely on the evaluators' summaries. These are targeted next-response checks and short state transitions, not a continuous 100-turn interview.

| Cases | Observed behavior | Final scoped result |
| --- | --- | --- |
| I1 | Starts one question at the default count for a supplied brand. | Passed |
| I2 | Pauses without issuing another question; preserves answers, unknown and skip. | Passed |
| I3 | Resumes the same pending follow-up without requiring the full old archive. | Passed |
| I4, repeated | Resolves Q10, records 7 answered / 2 unknown / 1 skipped, distinguishes older checkpoint-reported progress, then asks Q11. | Passed in current-instruction retest |
| I5 | Requests correction of conflicting answered/pending state without advancing. | Passed |
| I6 | Stops at an explicit four-question pilot target; produces a provisional guide, actual archive and honest counts. | Passed |
| G1 | Produces an early guide from checkpoint summaries without inventing raw replies or operational details. | Passed |
| G2, repeated | Challenges unsupported strategic preference, compares founders by theme, labels summary-based conflicts tentative and requests relevant excerpts. | Passed in current-reference retest |
| G3, repeated | Identifies the missing founder perspective and cites available summary evidence explicitly. | Passed in current-reference retest |
| G4 | Drafts useful examples while withholding unsupported outcome and customer-sentiment claims. | Passed |
| C1 | Incorporates a newer Q11 reply and continues at Q12 rather than following the stale checkpoint prediction. | Passed |
| C2 | Changes target to 80, preserves a late Q18 revision and continues the pending Q45 follow-up. | Passed |
| C3 | Avoids treating two acquisition-channel summaries as a definitive strategic conflict or an approved combined plan. | Passed |

The initial I4 output lacked an explicit checkpoint-reported label. The original G2/G3 outputs used abbreviated summary provenance, and G2 treated summary-based conflicts as definitive. These version-scoped gaps prompted clearer instructions. The original outputs remain in the evidence; affected cases were repeated under the updated instructions. The repeated results do not establish a universal fix across all possible inputs.

Raw evidence:

- [Interview and continuity outputs](tests/interview-results.md)
- [Guide and comparison outputs, including reruns](tests/guide-results.md)
- [Fresh I4 checkpoint retest](tests/checkpoint-retest.md)

Machine-specific source paths have been normalised in the portable reports; the captured reply text is preserved. All fixtures and replies are fictional. No real founder interview or customer record is included.

## Council review

Codex, Claude and Grok challenged the design and agreed after revisions concerning visible-state precedence, summary provenance, tentative disagreement and aspiration versus current delivery. This was a design review, not evidence that the advisers completed a 100-question interview or verified a business claim.

## Limits

- No real 100-question interview or ten-checkpoint lifecycle has been completed.
- Cross-session persistence and host-specific skill import/installation are not established by a text checkpoint response.
- Customer demand, brand alignment and social content effectiveness are not validated by these tests.
- External council tools are optional. Their availability and permissions in another user's host are not guaranteed.
- A complete verbatim archive still requires actual transcript blocks, even when a compact checkpoint supports continuation.
