# Dataset Name ($\mathbb{DS}_{4}^\mathsf{trace}$): randomized_positive_negative_trace.csv

# Dataset source: Derived from using NuSMV Model Checker

# Dataset used for Task: Trace Classification

# Dataset Size: 306 unique formulas, yielding 612 traces (positive + negative)

# Dataset Format: CSV


The dataset contains pairs of LTL formulas and NuSMV-generated traces, labeled as either satisfying (positive) or violating (negative) the formula.

The dataset is a comma-separated list of the following quadruples:
(LTL Formula String, Trace String, Trace Label, AP Mapping)

- **LTL Formula String:** The LTL formula for which the trace was generated.
- **Trace String:** The execution trace (sequence of states) in a NuSMV-compatible format.
- **Trace Label:** A binary label: "positive" (satisfies the formula) or "negative" (violates the formula).
