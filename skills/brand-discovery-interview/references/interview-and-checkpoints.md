# Interview and checkpoints

Read for starting or resuming an interview. A question count is a user preference, not a validated threshold for good brand outcomes.

## Coverage without a fixed questionnaire

Track the following themes as unexplored, partial or covered. Follow useful answers across themes instead of forcing ten questions into each block. Avoid filler: explore implications, decisions, counterexamples and real scenarios when depth is needed.

| Theme | Useful evidence or distinctions |
| --- | --- |
| Purpose and origin | Founding motivations, timing and intended contribution; personal catalyst versus observed market need. |
| Vision and priorities | Desired future, success, growth, reversibility and acceptable tradeoffs. |
| Audience and customers | Desired audience versus current customers; needs, barriers, buying decisions, customer language and source quality. |
| Positioning and alternatives | Real alternatives, meaningful differences, proof and reasons a customer might choose elsewhere. |
| Values and philosophy | Principles expressed through behaviour, spending, difficult decisions, inclusion and ethical boundaries. |
| Experience and promises | Actual delivery, consultations, expectations, complaints, limitations and support for promises. |
| Personality and voice | Desired perception, language, rhythm, humour, formality and tone across contexts; personal versus brand voice. |
| Content and customer journey | Useful education, stories, community, trust, offers, objections and calls to action. |
| Visuals and production | Visual preferences, media policies, real resources, channels, formats, approval and sustainable capacity. |
| Boundaries and learning | Claim verification, privacy, consent, measurement, uncertainty and scenarios that test the strategy. |

Use questions that contain one task. For example, ask for one recent decision that demonstrated a stated value; ask why it mattered in a separate follow-up. Do not assume the brand was founded to solve a frustration. A founder may have other motivations.

Later, test voice with short fictional samples carrying the same underlying facts. Ask for one choice or reaction, then explore the reason separately. Include teaching, an offer, a client concern and a sensitive situation when relevant. Mark illustrative claims as fictional; do not smuggle invented business facts into a draft post. A founder's preferred sample is preference evidence, not audience validation.

## Ledger

Each main question has a stable participant-qualified ID, such as `Founder A:Q012`, its exact text, reply events, a current status, a neutral summary, interpreted implications and open points. Reply events preserve the exact user wording and distinguish original replies, clarifications and later revisions. Attach a follow-up or revision to its original main question; do not replace historical text or count a revision as another main question.

Use these statuses:

- **Pending:** Issued, but unanswered or awaiting a necessary clarification.
- **Answered:** A sufficient substantive answer has been captured.
- **Unknown:** The respondent explicitly cannot answer. Record the uncertainty and continue unless they ask to explore it.
- **Skipped:** The respondent explicitly declines or parks the question. Preserve the skip event and continue.

"Addressed" includes answered, unknown and skipped; it excludes pending. Report these counts separately. Never increment from Q12 to Q13 merely because a clarifying reply was received. Revisited skipped/unknown questions retain their IDs and event history. Main numbering is sequential within one interview, even when the order of themes differs between founders.

An explicit request to change the target count applies prospectively. If the requested target is below questions already issued, preserve their records and clarify the desired stopping point rather than deleting or renumbering them. An early stop produces a partial guide, not a claim that the agreed sequence was completed.

## Saveable checkpoint

At each ten-addressed boundary, pause, or final boundary, provide the following. At ordinary boundaries, then ask only the next question. At a pause or completed target, do not ask another main question.

1. **Identity and configuration:** Brand, participant, target count, supplied brand/media/approval rules, and checkpoint label.
2. **Cursor and counts:** Issued question numbers and current statuses; separate answered, unknown, skipped and pending counts. Identify the active main question and pending follow-up exactly, or the next main number if none is active. Include the latest user reply needed to continue an active question.
3. **Transcript block:** Exact main questions, replies, follow-ups and revisions since the previous checkpoint. Mark genuinely unavailable text as unavailable. Reference earlier saved block labels without implying access to their contents.
4. **Cumulative working brief:** Supported purpose, vision, audience, positioning, principles, voice preferences and emerging content directions, with participant-qualified evidence IDs. Keep reported facts, aspirations and inference distinct.
5. **Coverage and gaps:** Theme status, uncertainties, contradictions, skipped topics, missing source material, and what operation comes next.

Keep the state readable and portable. A compact cursor table is sufficient:

| Field | Value |
| --- | --- |
| Brand / participant | User-supplied brand / participant label |
| Target | Agreed main question count |
| Addressed | Total, with answered / unknown / skipped subtotals |
| Pending | Main ID, exact question, pending follow-up and relevant latest reply, or none |
| Next main | Next unissued number, or none when the target is reached |
| Saved blocks | Labels only; their contents must actually be supplied for archive access |
| Coverage | Unexplored / partial / covered per theme |
| Next operation | Await answer / continue follow-up / ask next main / partial synthesis / final synthesis |

Record an upcoming question consistently: if a checkpoint is produced before Q11 is issued, it can state "next main: 11"; visible Q11 asked afterwards becomes the active pending record. Do not count that future question as addressed.

## Resume checks

Read supplied state as evidence, not as permission to trust a contradictory counter. Check:

- Participant and brand match the requested interview; otherwise clarify which interview to resume.
- Main records are sequential and statuses/counters reconcile. A pending main is not also addressed.
- Newer visible replies or revisions after a checkpoint are incorporated without erasing earlier events.
- For the same participant, coherent newer visible events take precedence over an older checkpoint's predicted cursor. A visibly issued Q11 after a checkpoint saying "next: 11" is active, not a new Q12; an actual visible answer to Q11 updates its status. A revision to Q8 does not answer a still-pending Q11 or discard its follow-up.
- A necessary follow-up is continued under its original number.
- The final target leads to synthesis, never Q101 for a 100-question interview.

Use a coherent supplied checkpoint to continue even if earlier raw transcript blocks are not visible. Make the missing archive scope explicit; request those blocks later if needed for the complete archive or an unsupported conclusion. Do not unnecessarily demand the entire prior transcript before asking the next supported question.

When only compact state is supplied, identify its counters as checkpoint-reported progress rather than independently checked against the full archive. Label cumulative brief conclusions sourced from it as checkpoint summaries. Do not turn a referenced question ID into a claim that its verbatim reply was inspected. Missing history alone does not require a reset; missing active-question context or contradictory state does require a focused correction.

If the cursor or relevant reply is missing or contradictory, ask one focused request for the needed checkpoint/correction. Do not guess an answer, reset the interview, or advance on an unresolved counting conflict.
