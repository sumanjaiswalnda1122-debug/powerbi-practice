# Power Query Error Cleaning Practice

Practicing common **Power Query (Get & Transform)** data-cleaning techniques in Power BI, using a messy mock sales dataset.

## Dataset
A sample "Orders" table (`power_query_errors_practice.xlsx`) containing intentional data-quality issues:
- Duplicate Order IDs
- Blank/missing values (CustomerName, City, OrderDate)
- Inconsistent text casing and extra spaces (" PRIYA", "pune")
- Numbers stored as text (e.g. "five thousand")
- Inconsistent placeholders for missing data ("NA")
- Duplicate spacing in product names ("Advanced  Excel")

## What I practiced
| # | Issue | Technique Used |
|---|-------|----------------|
| 1 | Duplicate OrderIDs | Remove Rows → Remove Duplicates |
| 2 | Blank CustomerName/City | Replace Values (null → "Unknown") |
| 3 | Extra spaces & inconsistent case | Trim, Clean, Capitalize Each Word |
| 4 | Text stored as numbers / errors | Change Type → Replace Errors with 0 |
| 5 | Inconsistent product naming | Replace Values |
| 6 | Missing OrderDate | Filter → Remove blank rows |
| 7 | "NA" placeholder in Discount | Replace Values ("NA" → 0) |

## Files
- `error_solve.pbix` — Power BI file with the cleaning steps applied in Power Query
- `power_query_errors_practice.xlsx` — source data, plus the practice questions and suggested solution steps

## Skills demonstrated
Power Query fundamentals: Remove Duplicates, Replace Values, Trim/Clean, Data Type conversion, Error Handling, Filtering.
