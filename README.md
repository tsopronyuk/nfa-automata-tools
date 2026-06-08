# NFA Automata Tools

Tools for generating, visualizing, and determinizing finite automata for educational purposes.

## Features

- Generate random nondeterministic finite automata (NFA) with guaranteed state reachability
- Visualize automata as transition diagrams (SVG/PNG)
- Pairwise display for concatenation and union operations
- Generate 20+ individual assignment variants for students
- Determinization algorithm (NFA → DFA) with reachable state analysis

## New: Moodle Test Generator

A new tool `generate_tests.ipynb` has been added to automatically generate ready-to-use quizzes for Moodle.

### Features
- Generates up to 100 unique variants
- Exports to Moodle XML format with embedded diagrams
- Permutation-tolerant grading (accepts any order of Σ symbols and transitions)
- Automatic answer calculation for all four operations

### Usage
1. Run `generate_tests.ipynb` in Google Colab or Jupyter
2. Download the generated `finite_automata_100_variants.xml`
3. Import into Moodle (Question bank → Import → Moodle XML format)
4. Create a quiz with random questions from the imported category

### Files
- `generate_tests.ipynb` - Main notebook for test generation
- `finite_automata_100_variants.xml` - Example output (100 variants)
- `instructions/student_instructions.html` - Student instruction sheet

## Requirements

- Python 3.7+
- graphviz
- IPython
- Jupyter Notebook (optional)

## Installation

```bash
pip install graphviz ipython
