# Dataset Name: nl2pl_finalized.csv

$\mathbb{DS}_{3}^\mathsf{prop}$

# Dataset source: Curated from Textbooks, Real-World Scenarios, and Problem Sets

# Dataset used for Task: Atomic Proposition Extraction

# Dataset Size: 144

# Dataset Format: CSV

This dataset is curated to evaluate the LLMs' capability to identify and extract relevant atomic propositions from natural language descriptions and map them to atomic variables.

The dataset is a comma-separated list of the following triples:
(natural language sentence, ground truth propositional logic formula (though not used), atomic proposition mapping)

- **natural language sentence:** The English text describing a logical condition.
- **ground truth propositional logic formula:** The correct propositional logic formula for the sentence.
- **atomic proposition mapping:** A string or list defining the mapping of natural language fragments to their corresponding propositional variables.

