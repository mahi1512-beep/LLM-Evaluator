# LLM Response Quality Evaluator

An **RLHF-style annotation pipeline** for evaluating and ranking AI-generated responses across 5 quality dimensions — simulating real-world data annotation work used at platforms like Scale AI, Appen, and Outlier AI.

## What This Project Does

- Annotates **500+ AI response pairs** across 4 domains (general knowledge, coding, math, safety)
- Scores each response on **5 quality dimensions**: Accuracy, Helpfulness, Coherence, Safety, Completeness
- Generates **RLHF preference pairs** (chosen vs rejected) for model fine-tuning
- Achieves **92% inter-rater consistency** — above the 85% industry benchmark
- Exports training-ready datasets in CSV and JSON format

## Quality Dimensions

| Dimension | Description |
|-----------|-------------|
| Accuracy | Is the response factually correct? (1–5) |
| Helpfulness | Does it fully address the user's need? (1–5) |
| Coherence | Is it clear and well-structured? (1–5) |
| Safety | Does it avoid harmful content? (1–5) |
| Completeness | Does it cover all parts of the prompt? (1–5) |

## Project Structure

```
llm-evaluator/
├── llm_evaluator.ipynb       # Main annotation notebook
├── annotated_responses.csv   # Exported annotation results
├── rlhf_preference_pairs.json # RLHF-ready training data
├── annotation_analysis.png   # Visualization of annotation results
└── requirements.txt
```

## Setup

```bash
pip install -r requirements.txt
jupyter notebook llm_evaluator.ipynb
```

## Results

- 500 response pairs annotated across 4 domains
- 200 RLHF preference pairs exported for fine-tuning
- 92% inter-rater consistency (industry benchmark: 85%)
- Preference distribution: ~65% Response A preferred, ~35% Response B

## Skills Demonstrated

- RLHF annotation pipeline design
- Multi-dimensional quality rubric development
- Preference pair generation for LLM training
- Inter-rater consistency measurement
- Data export in ML-ready formats (CSV, JSON)

## Author

**Mahendra Singh** | [LinkedIn](#) | mahendrasingh854239@gmail.com
