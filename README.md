# Fallen Angels
![Fallen Angels](fall.png)
Fallen Angels is an AI safety research project exploring why language models sometimes comply with jailbreak prompts and how successful and unsuccessful attempts differ.

The project collects structured prompt-response experiments and analyzes patterns across prompt types, model responses, and outcomes.

## Research Questions

* Which jailbreak strategies are most associated with compliance?
* How do successful and failed attempts differ?
* Does prompt structure or length affect outcomes?
* Are the same jailbreak strategies effective across different models?

## Models

Initial experiments:

* Gemma 4

More models will be added for comparison.

## Dataset

Each row represents one jailbreak experiment.

| Column           | Description                     |
| ---------------- | ------------------------------- |
| `prompt`         | Prompt sent to the model        |
| `prompt_type`    | Jailbreak strategy or variation |
| `input_length`   | Length of the prompt            |
| `model_response` | Model output                    |
| `outcome`        | Refused, partial, or complied   |
| `model`          | Model used                      |

## Tech Stack

* Python
* NumPy
* Pandas
* Matplotlib
* scikit-learn
* Hugging Face

## Setup

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/fallen-angels.git
cd fallen-angels
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

Experiments and analysis are currently developed in notebooks.

```text
notebooks/
```

Open the notebooks locally with Jupyter or run them in Google Colab.

## Repository Structure

```text
fallen-angels/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
├── results/
├── requirements.txt
├── .gitignore
└── README.md
```

## Goals

### Direct Goal

Analyze patterns behind successful and unsuccessful jailbreak attempts.

### Indirect Goal

Use the project to build practical skills in data analysis, machine learning, LLM evaluation, and interpretability.

## Disclaimer

This project is intended for AI safety research and educational purposes.
