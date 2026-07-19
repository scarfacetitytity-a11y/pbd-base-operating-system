---
name: trade-journal
description: Log a completed trade into the trading journal using the Identity Rewire template. Use when the user says they just closed a trade, wants to journal a trade, log a result, or do a post-trade review. Appends a structured entry to trading/journal/entries.md.
---

# Trade Journal

Reference: `trading/psychology_suite.md` (Post-trade Decompression + Identity Rewire).

## Steps

1. Ask for whatever the user hasn't already given:
   - Instrument (XAUUSD/US30/US100/GBPUSD/other)
   - Trade result (win/loss/breakeven, R multiple or £/$ if known)
   - Rules followed
   - Rules broken (if any — don't let "none" pass without a quick sanity check)
   - Emotion before entry
   - Emotion during trade
   - Emotion after exit
   - What was the setup (tie back to Sniper v1.0 if relevant: HTF bias, liquidity sweep, M5/M1 confirmation)
   - Lesson
   - Identity statement (what identity did this trade reinforce — disciplined trader or impulsive one?)
   - Next trade correction

2. If `trading/journal/entries.md` doesn't exist, create it with a `# Trade Journal` heading.

3. Append a new dated entry at the bottom in this format:

```
## YYYY-MM-DD — INSTRUMENT — RESULT

Setup:
Rules followed:
Rules broken:
Emotion before entry:
Emotion during trade:
Emotion after exit:
Lesson:
Identity statement:
Next trade correction:
```

4. Don't rewrite or edit past entries. Journal is append-only — it's a record, not a draft.

5. Keep the tone honest and direct. If rules were broken, say so plainly rather than softening it — the point of the journal is accuracy, not comfort.
