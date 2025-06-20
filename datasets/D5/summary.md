# Dataset Name: past_ltl.csv

$\mathbb{DS}_{5}^\mathsf{pastltl}$

# Dataset source: Adapted from $\mathbb{DS}_{1}^\mathsf{tricky}$ (rephrased)

# Dataset used for Task: Natural Language to Past Linear Temporal Logic (PastLTL) Translation

# Dataset Size: 294

# Dataset Format: CSV

This dataset was created by adapting the natural language specifications from the $\mathbb{DS}_{1}^\mathsf{tricky}$ dataset. The original future-oriented natural language was rephrased to utilize past temporal expressions, and the corresponding ground truth LTL formulas were converted to include Past LTL operators.

The dataset is a comma-separated list of the following triples:
(natural language, ground truth PastLTL formula, atomic proposition mapping)

- **natural language:** The English text describing a past temporal property.
- **ground truth PastLTL formula:** The corresponding LTL formula using past temporal operators.
- **atomic proposition mapping:** A string or list defining the mapping of natural language fragments to their propositional variables.

**Purpose:** This dataset specifically supports the assessment of LLMs’ translation capabilities to past-time temporal logic, exploring their understanding of operators like Yesterday (Y), Once (O), Historically (H), and Since (S).