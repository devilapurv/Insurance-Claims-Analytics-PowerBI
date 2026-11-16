# Data Cleaning Notes

Original dataset: 1,000 rows, 39 columns.

- Source CSV contains 91 missing `authorities_contacted` values.
- Several categorical columns use `?` to indicate unknown/missing information.
- Missing categorical entries and question-mark placeholders were converted to `Unknown`.
- Text values were stripped of surrounding whitespace.
- `policy_bind_date` and `incident_date` were standardized to ISO dates.
- No claims were deleted, and no numeric claim amounts were changed.
- The original CSV is preserved unchanged.

These are documented portfolio-cleaning steps; they should not be represented as a verbatim export of Power BI Power Query transformations.
