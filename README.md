# Project-Sales-Performance-Report
Use DataFrames, Series, row selection, filters, column operations, groupby and merges in one report.

Create a sales performance report for the supplied team. Calculate totals, filter reps who met quota and summarize results by region. The three parts carry code forward.

This project turns table operations into a report. Start by deciding what one row represents, then make sure your filters and grouping keys use that same level. A sales table may have one row per order while the final question asks for one result per region or product.

Build the report in visible stages. Inspect the source table, select the columns you need, filter invalid or irrelevant rows, create any derived values and aggregate at the level required by the question. Keeping those stages separate makes a wrong total easier to trace. A polished table is not enough if the grouping level or join logic changed what the numbers mean.

The report combines selection and presentation patterns. df.loc[row_label, 'Sales'] selects a labeled value, while idxmax() returns the index label of the row containing the largest value. Use .round(1) for one decimal place, iterrows() when a report must format one row at a time, and f-string formats such as f"${amount:,.0f}" for readable currency.

Build the sales DataFrame and print a quick summary: total reps, total sales, average sales, and the top performer's name.
In this part you will

Create a DataFrame from the dictionary provided in the starter code
Print the number of reps using len(df)
Print the total and average sales formatted with commas and a $ sign
Print the name of the rep with the highest Sales value
Example output

Total reps: 6
Total sales: $477,000
Average sales: $79,500
Top performer: Frank
