 ## AI Reads AI: Let Large Language Models Analyze Kaggle's Best
Using LLMs to Summarize, Classify, and Visualize High-Impact Kaggle Notebooks

---

## Introduction

Kaggle notebooks are a goldmine of applied AI knowledge—but understanding hundreds of them is overwhelming. “**AI Reads AI**” is a lightweight, local-first project that uses **open-source LLMs** to automatically summarize and classify Kaggle's top notebooks from the Meta Kaggle dataset.

The vision is simple: **let AI read AI**—and make Kaggle’s collective knowledge more accessible for everyone.

---

## Approach

We use:
- The **Meta Kaggle and Meta Kaggle Code** datasets to extract notebook content
- Open-weight LLMs like **Gemma** or **Mistral** to summarize notebook code and markdown
- Prompt engineering to classify each notebook (Tree-based, Deep Learning, NLP)
- **Bokeh** for interactive dashboard visualizations

---

## Pipeline Overview

1. Parse notebook `.ipynb` cells into code/markdown
2. Feed structured prompt into a lightweight local LLM
3. Receive a summary + category classification
4. Store results as JSON
5. Visualize summary and topic distributions with interactive plots

---

## Results & Insights

- Majority of high-voted notebooks used **Tree-based models** for tabular data
- **CNNs** and **Transformers** dominate image and text challenges
- Notebook summaries by LLMs are concise and often comparable to human-written descriptions

---

##  Technical Note

Due to hardware limitations (standard laptop with no GPU), the current pipeline:
- Uses a small subset of Meta Kaggle notebooks
- Relies on quantized or low-weight models
- Prioritizes clarity and reproducibility

Despite this, the pipeline is functional, and easily portable to larger LLMs or cloud runtimes.

---

## Supplementary Files

- `llm_generated_summaries.json`: AI-generated summaries of Kaggle notebooks
- `kaggle_llm_dashboard.html`: Bokeh dashboard for model-type distribution
- Kaggle Notebook (WIP): to be published publicly by submission

---

Kaggle is the world's most valuable playground for real AI work—and this project is my small contribution to making it even more useful.

While working locally with limited resources, I built a working prototype that:
- Parses and summarizes high-quality notebooks using LLMs
- Classifies them by strategy
- Visualizes these insights in a clean dashboard

The idea is scalable, useful, and community-oriented

## By Navroop dhillon
