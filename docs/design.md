# Design Notes

Objective
- Summarize A/B test outcomes and flag regressions.

Data flow
- Load JSON dataset
- Validate each record against rules and categories
- Compute totals, averages, and top-ranked items
- Render a report with key metrics and issues

Validation rules
- lift must be between min and max
- confidence_score must be 0 to 100
- Category must be one of the configured categories
- Status must be one of the allowed statuses

Extension ideas
- Add CSV import/export
- Add trend comparisons across multiple datasets
- Add thresholds for alerts per category
