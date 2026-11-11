1 — Attempt Before AI (no AI used in this section)

File snapshot & integrity

- Original file: `teaching_prices_messy.csv`
- SHA-256 of original: `[PASTE OUTPUT OF: sha256sum teaching_prices_messy.csv]`
- Commit message: `attempt-before-AI`
- Working copy for cleaning: `teaching_prices_copy.csv` (original never edited)

> Gate 1 satisfied: hash recorded and committed before any AI contact.

How I loaded it (in-class tools only)

python
import pandas as pd, hashlib
raw = pd.read_csv("teaching_prices_messy.csv", dtype=str, keep_default_na=False)
print(raw.shape)
print(raw.head(10))
print(raw.dtypes)
print(raw.isna().sum())
print(raw.describe(include="all"))
for c in raw.columns:
    print(c, raw[c].nunique(), raw[c].unique()[:20])
print("dupes:", raw.duplicated().sum())
