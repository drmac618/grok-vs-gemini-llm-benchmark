# Grok vs Gemini LLM Benchmark

This project evaluates Grok and Gemini using a 100-prompt benchmark dataset.

## Evaluation Metrics

Responses were scored using a human evaluation rubric across four dimensions:

- Accuracy
- Clarity
- Completeness
- Safety

Scores use a 1–5 scale.

## Results

| Model | Overall Score |
|------|------|
| Gemini | 4.78 |
| Grok | 4.65 |

Gemini slightly outperformed Grok primarily due to higher factual accuracy.

## Repository Contents

dataset/  
- `benchmark_dataset.csv` — machine-readable benchmark dataset with metadata and `ExpectedAnswer`  
- `benchmark_dataset.json` — JSON version of the benchmark dataset  
- `grok_vs_gemini_llm_evaluation_single_reviewer_completed.xlsx` — full evaluation workbook

charts/  
Benchmark visualizations

`benchmark_results_report.md`  
Full benchmark report

`methodology.md`  
Evaluation procedure

## Dataset Schema

The benchmark dataset includes:

- PromptID
- Category
- TaskType
- Difficulty
- SkillTested
- GroundTruthAvailable
- Prompt
- ExpectedAnswer

Dataset format inspired by HELM, BIG-Bench, and OpenAI-style evaluation workflows.

## Purpose

This project demonstrates a small-scale LLM evaluation pipeline including:

- prompt dataset creation
- model response collection
- human evaluation scoring
- benchmark leaderboard generation
- performance visualization
- reproducible benchmark dataset design
