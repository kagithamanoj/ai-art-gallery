# 📊 Data Analysis & SQL Prompts

Prompts for data analysis, SQL queries, pandas, visualization, and reporting.

## SQL Queries

### Complex SQL Query
```
Write a SQL query for [database: PostgreSQL/MySQL] that:

Tables: [describe schema]
Goal: [what to retrieve]

Requirements:
- Use CTEs for readability
- Include proper JOINs
- Handle NULLs appropriately
- Add comments explaining complex logic
- Optimize for performance (explain index usage)
```

### Data Exploration Query Set
```
Generate a set of SQL queries to explore a new table called [table_name] with columns [list columns].

Include:
1. Row count and date range
2. Column-level statistics (min, max, avg, null %, distinct count)
3. Distribution of [categorical column]
4. Time series trend (daily/weekly/monthly)
5. Top N by [metric]
6. Anomaly detection (values outside 3σ)
7. Correlation between [col1] and [col2]
```

### ETL Pipeline SQL
```
Write SQL for an ETL pipeline that:
- Source: [source tables]
- Transformation: [business logic]
- Target: [destination table]

Include:
- Staging table creation with appropriate types
- Data quality checks (nulls, duplicates, range validation)
- Incremental load logic (only new/modified rows)
- Error logging table
- Idempotent design (safe to re-run)
```

## Python / Pandas

### DataFrame Analysis
```
I have a pandas DataFrame with these columns: [list columns with types]

Write Python code to:
1. [analysis task 1]
2. [analysis task 2]
3. [analysis task 3]

Use:
- Method chaining where possible
- Descriptive variable names
- Comments for complex operations
- Display results formatted nicely
```

### Data Cleaning Pipeline
```
Write a pandas data cleaning function for a dataset with:
- Columns: [list]
- Known issues: [missing values, outliers, duplicates, encoding issues]

The function should:
1. Remove exact duplicates
2. Handle missing values (strategy per column)
3. Fix data types
4. Standardize string formats (strip, lowercase, etc.)
5. Handle outliers (cap at percentiles or remove)
6. Validate against business rules
7. Return a summary of changes made
```

### Feature Engineering
```
Given a dataset with columns: [list columns]

Target: [target variable]

Generate feature engineering code that creates:
1. Date-based features (day of week, month, quarter, is_weekend)
2. Aggregation features (rolling mean, lag features)
3. Interaction features (ratios, products of key columns)
4. Encoding (one-hot for categoricals, target encoding)
5. Binning for continuous variables
6. Text features (if text columns: TF-IDF, word count, sentiment)

Use sklearn Pipeline for reproducibility.
```

## Visualization

### Dashboard Chart Descriptions
```
I need to create a [Matplotlib/Plotly/Seaborn] visualization for:

Data: [describe dataset]
Audience: [technical/executive/public]
Message: [key insight to convey]

Create code for:
1. Main chart (choose appropriate type)
2. Proper title, labels, and legend
3. Color scheme suitable for colorblind users
4. Annotations for key data points
5. Clean, publication-ready styling
```

### Exploratory Data Analysis Report
```
Write Python code for a complete EDA of this dataset: [describe]

Generate:
1. Shape, dtypes, memory usage
2. Missing value heatmap
3. Distribution plots for all numeric columns
4. Correlation matrix heatmap
5. Box plots for outlier detection
6. Pairplot for key features
7. Time series decomposition (if applicable)
8. Summary statistics table

Save all plots as PNGs and print a markdown summary.
```

## Reporting

### Executive Summary from Data
```
Analyze this data and write an executive summary:

[paste data or describe findings]

Format:
- TL;DR (one sentence)
- Key Metrics (3-5 bullet points with numbers)
- Trends (what's changing)
- Risks (what to watch)
- Recommendations (3 specific actions)

Tone: Concise, data-driven, actionable. No jargon.
Length: Under 300 words.
```

### KPI Dashboard Design
```
Design a KPI dashboard for [department/use case].

Metrics to track:
1. [metric 1 — definition and formula]
2. [metric 2]
3. [metric 3]

For each metric, specify:
- Visualization type (line, bar, gauge, number)
- Time granularity (daily/weekly/monthly)
- Comparison (vs. last period, vs. target)
- Alert thresholds (green/yellow/red)
- Data source
```
