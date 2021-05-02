# python_ml_benchmarks
Some system benchmarks for machine learning and deepl learning

Setup: You can use [poetry](https://python-poetry.org/docs/) for dependency management, then the pyproject.toml provides these. Else, you can install them separately for the test your interested in.

## xgboost
[Setup](https://pypi.org/project/xgboost/)

### tree benchmark

You can download or update the tree benchmarking script provided by xgboos via 
`curl https://raw.githubusercontent.com/dmlc/xgboost/master/tests/benchmark/benchmark_tree.py -o benchmark_tree.py`

Then you can run the benchmark via `python benchmark_tree.py --tree_method=hist` when running on CPU, or alternatively with the argument `--tree_method=gpu_hist` for running on gpu.

My personal results:
 - AMD Ryzen 7 4800H
	- tree_methood=hist:
		- Train Time: 19.940454959869385 seconds
