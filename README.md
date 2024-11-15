# Leo Chen Mini 10

[![CI](https://github.com/nogibjj/Leo_Chen_Mini_10/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/Leo_Chen_Mini_10/actions/workflows/cicd.yml)

## PySpark Data Processing
This project demonstrates the use of PySpark for processing and analyzing FIFA data. The main objectives include performing Spark SQL queries and data transformations to gain insights about global football viewership patterns, confederation distributions, and economic impacts.

### Data
[FiveThirtyEight FIFA Dataset](https://github.com/fivethirtyeight/data/blob/master/fifa)

This project uses FIFA countries audience dataset from FiveThirtyEight, which includes:
- Country names
- Confederation affiliations  
- Population share
- TV audience share
- GDP weighted share

### Key Features
1. Data extraction from source
2. Basic statistical analysis  
3. Confederation-based grouping and analysis
4. Regional categorization transformation
5. PySpark SQL queries

### Getting Started
1. Open codespaces
2. Wait for environment to be built
3. Run: `python main.py`
4. Check results in [PySpark Output Data/Summary](pyspark_output.md)

### Data Processing Flow
1. **Extract**: Download FIFA dataset using `extract()`
2. **Initialize**: Start Spark session via `start_spark()`
3. **Load**: Load FIFA data into DataFrame using `load_data()`
4. **Analyze**: Generate descriptive statistics via `describe()`
5. **Query**: Execute Spark SQL queries using `query()`
6. **Transform**: Perform regional categorization via `example_transform()`
7. **Cleanup**: End Spark session using `end_spark()`

### Output
After running the analysis, you'll get:
1. Basic statistics like mean and stddev
2. Confederation-wise country counts and average GDP shares
3. Regional categorization (Eurasia, Americas, Others)