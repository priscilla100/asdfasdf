# Dataset Name: book6_academic_ltl.csv

$\mathbb{DS}_{6}^\mathsf{book}$

# Dataset source: Curated from Formal Logic and Temporal Logic Textbooks & Academic Sources

# Dataset used for Task: Natural Language to Future Linear Temporal Logic (FutureLTL) Translation

# Dataset Size: 141

# Dataset Format: CSV

This dataset is a collation of LTL formulas and their natural language descriptions sourced from various textbooks and academic papers on formal logic and temporal logic. It contains natural language statements that often involve complex logical constructs, counterfactuals, necessity/possibility modalities, and real-world causality.

The dataset follows a similar structure to the Future LTL part of $\mathbb{DS}_{1}^\mathsf{tricky}$ and $\mathbb{DS}_{5}^\mathsf{pastltl}$.

The dataset is a comma-separated list of the following triples:
(natural language, ground truth FutureLTL formula, atomic proposition mapping)

- **natural language:** The English text describing a logical or temporal property.
- **ground truth FutureLTL formula:** The corresponding Future LTL formula.
- **atomic proposition mapping:** A string or list defining the mapping of natural language fragments to their propositional variables.

**Purpose:** The main goal of this dataset is to assess the practical applicability of LLMs in real-world scenarios where complex logical and temporal reasoning.