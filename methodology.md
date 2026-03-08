# Benchmark Methodology

## Prompt Dataset

The benchmark uses 100 prompts spanning several task types:

- factual knowledge
- mathematical reasoning
- reading comprehension
- instruction following
- troubleshooting tasks

A machine-readable dataset is included in both CSV and JSON formats.
Each benchmark item contains an `ExpectedAnswer` field to support reproducibility and future automated evaluation.

## Evaluation Process

Responses were scored by a single human reviewer using a rubric across four dimensions:

- Accuracy
- Clarity
- Completeness
- Safety

Each dimension uses a 1–5 scoring scale.

## Benchmark Goal

The goal of the benchmark is to compare the performance of Grok and Gemini across diverse tasks and visualize strengths and weaknesses using leaderboard and metric charts.

## Reproducibility Improvement

To align more closely with benchmark repositories such as HELM, BIG-Bench, and OpenAI-style evals, the project now includes:

- a machine-readable benchmark dataset
- prompt metadata
- an `ExpectedAnswer` column for reference-based evaluation
