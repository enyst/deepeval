---
name: repo
type: repo
agent: CodeActAgent
---
This repository contains the code for DeepEval, an open-source LLM evaluation framework. It is a Python library for evaluating and testing large language model systems.

## Repository Structure:
- `deepeval`: Core Python code for the DeepEval library.
- `docs`: Documentation website (Docusaurus).
- `examples`: Example scripts and use cases.
- `tests`: Unit and integration tests.
- `benchmarks`: Benchmark datasets and evaluation code.
- `integrations`: Integrations with libraries like Hugging Face, LangChain, LlamaIndex.
- `metrics`: Implementations of evaluation metrics.
- `red_teaming`: Red teaming and vulnerability scanning tools.
- `synthesizer`: Synthetic data generation functionality.
- `deepeval/cli`: Command-line interface.

## Testing:
- Tests are located in the `tests` directory.
- Uses Pytest framework.
- Run tests using the command: `deepeval test run tests/test_*.py` (or `deepeval test run <test_file.py>`).
- You can run tests in parallel using the `-n` flag: `deepeval test run tests/test_*.py -n <num_processes>`.
- Caching of test results is supported using the `-c` flag: `deepeval test run tests/test_*.py -c`.

## General Setup:
To set up the development environment:
1.  Create a virtual environment: `python3 -m venv venv`
2.  Activate the virtual environment: `source venv/bin/activate`
3.  Install dependencies: `pip install -U deepeval`