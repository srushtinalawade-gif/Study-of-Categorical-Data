# Study-of-Categorical-Data
## Name- Srushti J. Nalawade
## PRN- 25070123157
## Batch- A1
## Aim:
To investigate and implement a comprehensive suite of techniques for the analysis of categorical datasets using the Python Pandas library. This study focuses on executing frequency distribution, multi-dimensional cross-tabulations, and advanced data grouping to extract meaningful insights from non-numeric variables.
## Objectives

>Conceptual Distinction: Differentiate between Nominal (labels without inherent order) and Ordinal (labels with a logical scale or rank) data types.

>Distribution Analysis: Compute absolute frequency counts and relative percentage distributions for various categories.

>Relationship Mapping: Utilize Cross-tabulation (Crosstab) to identify correlations and overlaps between two or more categorical variables.

>Aggregation & Organization: Apply grouping mechanisms and sorting algorithms to structure data based on categorical attributes.

>Selective Extraction: Implement Boolean indexing and filtering to isolate specific subsets within a categorical framework.

## Theory
Categorical data consists of discrete values representing qualitative attributes rather than numerical measurements. In Pandas, these are often stored as object or category dtypes. Analyzing these variables is vital for identifying trends in data that cannot be summed or averaged.

### 1. Frequency Distribution & Proportions:
The foundational step in categorical analysis is determining the "weight" of each category.

>Frequency Counting: Identifying the raw number of occurrences for each label.

>Normalization: Converting counts into proportions ($\text{count} / \text{total}$). This provides a "Percentage Distribution," making it easier to compare datasets of different sizes.

### 2. Cross-Tabulation (Contingency Tables):

While frequency distribution looks at one variable, Crosstab looks at two. It generates a matrix (contingency table) that reveals how categories intersect. For instance, it can answer: "Do customers in the 'Premium' tier prefer 'Credit Card' payments more than 'Standard' tier customers?"

### 3. Diversity & Cardinality:

Understanding the "breadth" of the data involves:unique(): Extracting a list of all distinct labels present in a column.nunique(): Calculating the cardinality (the total count of unique categories), which helps identify if a column is high-cardinality (like names) or low-cardinality (like gender).

### Metadata and Exploration Techniques

>Value Counts (value_counts): The primary tool for tallying categories. It can be sorted by frequency or index to highlight dominant trends (e.g., identifying the top-selling product category).

>Percentage Analysis: By setting the normalize=True parameter, the output shifts from integers to decimals, allowing for statements like "The 'Electronics' department accounts for 35% of total inventory."

>Logical Filtering: Using conditional logic to "slice" the dataframe. For example, creating a sub-dataset that only contains 'Distinction' grade students to analyze their specific study habits.

>Advanced Categorical OperationsThe Crosstab Function: Beyond simple counts, pd.crosstab() can include "margins" (row/column totals) to provide a holistic view of the interaction between variables like 'Subscription Type' and 'Churn Status'.Data Grouping (groupby): This enables hierarchical analysis. By grouping by 'Department' and then counting 'Grades', we can see the specific performance distribution within each individual branch of an organization.

## Conclusion-

This experiment highlights that categorical analysis is the backbone of qualitative data science. Through the application of value_counts, crosstab, and groupby operations, we transform raw labels into actionable intelligence. The ability to visualize the relationship between variables—such as how specific demographics lean toward certain services—allows for data-driven decision-making that numerical averages alone cannot provide.
