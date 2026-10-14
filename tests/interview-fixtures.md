# Synthetic interview fixtures

All brands, replies and checkpoints below are fictional test data. Each case supplies a realistic request, not a claimed successful outcome.

## I1: Start

User request: Use the skill to start an independent brand interview for Maple Studio. Label me Founder A. Use the default length and ask one question at a time.

## I2: Pause after varied replies

Brand: Maple Studio. Participant: Founder A. Target: 100.

Visible conversation:

- Assistant, Q1: What was the original reason for starting Maple Studio?
- User: I wanted small businesses to get design work they could depend on.
- Assistant, Q2: What does dependable service look like to your clients?
- User: I don't know yet.
- Assistant, Q3: Which client group do you most want to serve?
- User: Skip this one for now.
- Assistant, Q4: What do you want clients to remember about working with you?
- User: Elegant work and straightforward communication. Pause here and save my progress.

Produce the next assistant response to the final user message.

## I3: Resume with a pending follow-up

User request: Resume Maple Studio using this checkpoint. I haven't answered the follow-up yet.

Checkpoint: Founder A; target 100; issued Q1-Q10. Answered: Q1, Q4, Q5, Q7, Q8, Q9. Unknown: Q2, Q6. Skipped: Q3. Pending: Q10. Earlier raw blocks are not currently supplied.

Active Q10: What should clients feel during the service experience?

Latest exact user reply: Premium.

Pending follow-up to Q10: What does premium mean in the service experience?

Cumulative working brief: The founder intends to serve small businesses with dependable design work, elegant outputs and straightforward communication. No customer evidence has been supplied. "Premium" is not yet defined. Coverage is partial.

## I4: Continue after the follow-up

Use I3 as the visible state. The assistant repeated its pending follow-up. User reply: Premium means they get scheduled progress updates and clear explanations of decisions, even when the work is delayed.

Produce the next assistant response. Earlier raw replies for Q1-Q9 are still unavailable.

## I5: Contradictory cursor

User request: Resume Maple Studio from my checkpoint.

Checkpoint: Founder A; target 100; Q1-Q10 are listed as answered. It also lists Q10 as pending with an unanswered necessary follow-up. Next main is listed as Q11. There are no newer replies to resolve the discrepancy.

Produce the next assistant response.

## I6: Target reached with an unknown and a skip

User request: Produce the guide from this completed short pilot interview.

Brand: Maple Studio. Participant: Founder A. Explicit target: 4.

- Q1: What was the original reason for starting Maple Studio?
- Reply: I wanted small businesses to get dependable design work.
- Q2: What evidence do you have about customers' preferred tone?
- Reply: I don't know yet.
- Q3: Which social platform should be the main focus?
- Reply: Skip this one.
- Q4: How should the brand sound when a deadline slips?
- Reply: Give a clear explanation, apologise briefly when it's our fault, and say what happens next.

No follow-up is pending. No customer evidence or channel performance is supplied.
