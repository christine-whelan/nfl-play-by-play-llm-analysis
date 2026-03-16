# NFL Play-by-Play Analysis using Python and LLMs

This project explores whether a Large Language Model (LLM) combined with Retrieval-Augmented Generation (RAG) can produce useful NFL scouting insights from play-by-play data.

The system compares a deterministic Python analysis pipeline with an LLM-based question-answering system.

## Project Goal

Traditional football scouting requires manually analyzing large amounts of play-by-play data. This project investigates whether an LLM-assisted system can quickly summarize opponent tendencies and generate strategic insights.

## Two System Approaches

### 1. Python Deterministic System
A traditional data analysis pipeline that computes exact statistics such as:

- run vs pass tendencies
- player usage
- formation frequency
- down-and-distance behavior
- situational tendencies

### 2. LLM + RAG System
A retrieval-augmented generation system that:

1. chunks play-by-play data
2. embeds the text
3. retrieves relevant plays
4. generates natural-language insights

This allows users to ask questions such as:

- "What are the Ravens' most common plays on 3rd and short?"
- "Which players are most targeted in the red zone?"
- "What tendencies appear in two-minute offense?"

## Evaluation

Both systems were evaluated on:

- Accuracy
- Completeness
- Specificity
- Response usefulness
- Speed

The deterministic Python system provided more reliable exact counts, while the LLM system was better at generating quick strategic summaries.

## Key Findings

The best approach is **not replacing traditional analytics with LLMs**, but combining both.

Python provides precise statistical grounding, while LLMs improve usability and exploratory analysis.

## Limitations

- Limited dataset scope
- Potential hallucinations in LLM responses
- Token/context limits
- Play-by-play data lacks full contextual game information

## Tech Stack

- Python
- Pandas
- Scikit-Learn
- Sentence Transformers
- LangChain
- Retrieval-Augmented Generation (RAG)
- Jupyter Notebooks

## Repository Structure
