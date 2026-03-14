skills:
  - name: load_dataset
    description: Reads the ward_budget.csv dataset, validates required columns, and reports rows where actual_spend is null.
    input: CSV file path containing the dataset.
    output: Loaded dataset and report of rows where actual_spend is null.
    error_handling: If file or required columns are missing, stop execution with an error message.

  - name: compute_growth
    description: Computes Month-over-Month growth for a specific ward and category.
    input: Dataset, ward name, category name, growth_type.
    output: Table containing period, actual_spend, growth_percentage, and formula used.
    error_handling: If growth_type is missing or invalid, refuse execution.
