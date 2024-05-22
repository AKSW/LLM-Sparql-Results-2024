# LLM-Sparql-Results-2024
temporary repository for publishing results on anonymous github. Will be moved to a permanent location later on.


## Results for 4 SPARQL SELECT query related task types:

* [SparqlSyntaxFixing](SparqlSyntaxFixing): Fixing syntax errors in SPARQL SELECT queries
* [Text2Sparql](Text2Sparql): Generate SPARQL SELECT queries from textual questions
* [Text2Answer](Text2Answer): Generate the answer for a textual question with a given knowledge graph
* [Sparql2Answer](Sparql2Answer): Generate the answer for a SPARQL SELECT query with a given knowledge graph


## Files generated for each run:

* result files generated, different serialization formats containing same information:
    * `llm-kg-bench_run-[YYYY-mm-DD_HH-MM-ss]_result.json`
    * `llm-kg-bench_run-[YYYY-mm-DD_HH-MM-ss]_result.yaml`
    * `llm-kg-bench_run-[YYYY-mm-DD_HH-MM-ss]_result.txt`
* model log containing all text sent between benchmark framework an LLM models: `llm-kg-bench_run-[YYYY-mm-DD_HH-MM-ss]_modelLog.jsonl`
* debug log with extensive log messages: `llm-kg-bench_run-[YYYY-mm-DD_HH-MM-ss]_debug-log.log`

## stats and plots generated per task
* csv/xlsx summary of all results for a task: `*.csv`/`*.xlsx`
* boxplot of all results for a task: `*boxplots*.png`

## other files:
* Benchmark framework configuration file used: `configuration-2024-05-sparql.yml`
* Count for all experiments per task and model combinations present in result files: `sparql6-boxplots__stats.csv`
* Logs of Matrix-Run executions generating the given result files: [`MatrixRun-Logs/`](MatrixRun-Logs/)

## repetition of evaluation with given result files:
* The Benchmarking framework supports the reevaluation of given result files via the `--reeval` parameter
