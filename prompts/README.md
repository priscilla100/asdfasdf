# Prompts Module

This module contains the meticulously crafted prompt templates used to query Large Language Models (LLMs) across various evaluation tasks in our study. Each `.py` file corresponds to a specific LTL-related task, providing the necessary instructions, syntax, semantics, and examples for the LLMs to perform the required translation or classification.

All prompt templates are defined as Python f-strings (or multi-line strings with placeholders) to allow for dynamic insertion of natural language inputs or previous LLM responses during the evaluation process.

**`BASE_INSTRUCTIONS`** is a comprehensive explanation of the target task, the definition of propositional variables, logical connectives, and temporal operators.
    

## Full Prompt Templates
* **`ZERO_SHOT_PROMPT_TEMPLATE`**: Combines `BASE_INSTRUCTIONS` and `TASK_SPECIFIC_INSTRUCTIONS`.
* **`FEW_SHOT_PROMPT_TEMPLATE`**: Combines `BASE_INSTRUCTIONS`, `FEW_SHOT_EXAMPLES`, and `TASK_SPECIFIC_INSTRUCTIONS`.
* **`SELF_REFINE_PROMPT_TEMPLATE`**: Combines `BASE_INSTRUCTIONS`, `TASK_SPECIFIC_INSTRUCTIONS`, and includes a placeholder for the LLM's previous response for iterative refinement.

## Prompt Files Overview:

* **`nl2ltl_prompt_template.py`**: Prompts for Natural Language to **Future LTL** formula translation.
* **`nl2pastltl_prompt_template.py`**: Prompts for Natural Language to **Past LTL** formula translation.
* **`nl2pl_prompt_template.py`**: Prompts for Natural Language to **Propositional Logic** formula translation (used for Atomic Proposition Extraction task).
* **`trace_generation_prompt_template.py`**: Prompts for LLMs to **generate execution traces** from LTL formulas.
* **`trace_characterization_prompt_template.py`**: Prompts for LLMs to **classify traces** (satisfying/violating) for a given LTL formula.
* **`wff_prompt_template.py`**: Prompts for LLMs to classify if an LTL formula is **well-formed** or not.

These prompt templates are consumed by the main evaluation scripts located in the `experiments/` directory to generate API requests to various LLM providers.
