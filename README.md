%%writefile README.md
# Netflix Data Cleaning Report

## Changes Made:
1. **Missing Values**:
   - Dropped columns `director` and `cast` (high null counts).
   - Filled `country` with "Unknown" and `rating` with mode (most common value).
2. **Duplicates**: Removed 0 duplicate rows.
3. **Standardization**:
   - Dates: Converted `date_added` to datetime format.
   - Text: Cleaned `title` (title case) and `rating` (removed hyphens).
4. **Column Names**: Formatted to lowercase with underscores (e.g., `show_id`).

## Tools Used:
- Python (Pandas) in Google Colab.

## Files:
- [cleaned_netflix_titles.csv](cleaned_netflix_titles.csv)
