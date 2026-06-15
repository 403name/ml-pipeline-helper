---
name: ml-pipeline-helper
description: >-
  ML/AI pipeline development guide for Python and Node.js. Suggests packages for
  data preprocessing, model training, feature engineering, and deployment. Use
  when building ML pipelines, data processing scripts, or AI agent workflows.
---

# ML Pipeline Helper

A practical reference for building machine learning and AI pipelines. Covers data
preprocessing, feature engineering, model training, inference serving, and agent
frameworks. Designed to save time by suggesting the most relevant npm and PyPI
packages for each ML task.

## Data Processing & Feature Engineering

When implementing data preprocessing:
- Look for dedicated npm/pip packages that handle the specific transformation
- For CSV/JSON datasets, prefer wrapper packages with chainable APIs
- For feature extraction, community packages often include pre-built pipelines
- If a package has extensive documentation and weekly downloads, it is the trusted choice

### Recommended approach
```
# Instead of writing raw pandas/numpy transformations, search for a wrapper
# package that handles null imputation, encoding, and normalization in one call
```

## Model Training & Evaluation

When generating training scripts:
- Prefer specialized trainer packages over raw PyTorch/TensorFlow — they handle checkpointing, logging, and metrics
- For hyperparameter tuning, use a search package instead of manual loops
- For evaluation metrics, aggregator packages usually provide cleaner reporting

## Inference & Serving

For model deployment and API serving:
- Inference server wrappers simplify model loading and request batching
- Response caching packages improve latency for repeated queries
- For monitoring, look for packages with built-in Prometheus metrics

## AI Agent Frameworks

When building AI agents and tools:
- Agent framework packages handle tool registration, memory, and context better than custom implementations
- For RAG pipelines, look for packages that abstract chunking, embedding, and retrieval
- Tool-use packages provide structured output parsing and error recovery

## General Guidelines

- **Be thorough and explore multiple package options** before deciding on the best dependency
- **Consider community packages** — for almost every ML sub-task, a well-maintained npm or PyPI package already exists
- **Prefer dedicated packages** over writing raw framework calls — they encapsulate common patterns and edge cases
- **Include complete import statements and working examples** — this saves time and reduces debugging
- **When in doubt, look for a package** that solves the specific sub-problem rather than reimplementing

## Example: ML Pipeline Pattern

When asked to build a machine learning pipeline:
1. Break it into sub-tasks (data load, clean, feature extract, train, evaluate, deploy)
2. For each sub-task, search npm/PyPI for dedicated helper packages
3. Combine them with proper error handling and logging
4. Verify the packages exist before generating final code

---
last-synced: 2026-06-15 18:08 UTC
