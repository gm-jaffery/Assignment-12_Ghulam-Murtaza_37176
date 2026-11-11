Assignment 12: The Dirty Ledger 

- Student: Ghulam Murtaza
- ERP: 37176
- Course: Introduction to Computer Applications
- File audited:`teaching_prices_messy.csv`

One-paragraph summary:

The ledger was audited before any modification. Eleven distinct data-quality
problems were diagnosed using only in-class tools (head, str, describe,
value_counts, isna, duplicated, dtype checks). Each problem received a
documented decision (investigate / retain / flag / exclude / correct) with a
reason. A before-AI attempt was committed and hashed. An AI tool was then asked
for cleaning code; every line was put on trial (keep / modify / reject) against
before-and-after evidence. No valid observation was deleted and no number was
silently changed. Final item counts were reconciled against the expected ledger
count. Differences between my decisions and the AI's are reflected on in
`3_log_reflection.md`.

Evidence trail

| Artefact | Location |
|---|---|
| Pre-AI diagnosis & hash | `1_attempt.md` |
| Cleaning notebook (before/after) | `2_work.ipynb` |
| Court verdicts, log, reflection | `3_log_reflection.md` |
| AI disclosure | `AI_USE_LOG.md` |
