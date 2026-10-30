# Survey Feedback Analysis (Python)

A beginner-friendly Python project that collects, cleans, and analyzes customer survey feedback using core Python only: dictionaries, lists, sets, loops, functions, and built-ins like `zip()`, `sorted()`, and `enumerate()`.

## Overview

The project starts with 10 sample feedback entries, lets the user add new ones through the console (with rating validation), cleans the free-text comments, and then produces summary insights such as the average rating, keyword counts, and a ranked list of feedback.

## Features

- **Data entry**: store feedback in a dictionary with `S_No`, `Name`, `Feedback`, and `Rating`
- **Interactive input**: add any number of new feedback entries via `input()`
- **Input validation**: ratings outside 1 to 5 are rejected and re-requested
- **Text cleaning**: removes punctuation, trims extra whitespace, and converts to lowercase
- **Keyword counts**: reusable function that counts feedbacks containing a given word
- **Summary insights**:
  - Average rating
  - Longest comment
  - Unique words across all feedback
  - Feedback sorted by rating (highest to lowest)

## Data Structure

```python
feedback_data = {
    'S_No':     [1, 2, 3, ...],
    'Name':     ['Ravi', 'Meera', ...],
    'Feedback': ['Very GOOD Service!!!', 'poor support, not happy', ...],
    'Rating':   [5, 2, ...]
}
```

## Workflow

1. **Data entry**: load the sample data and append new user-entered feedback
2. **Data cleaning**: normalize every comment (punctuation removed, lowercase, single spaces)
3. **Word count insights**: count feedbacks containing "good", "poor", and "excellent"
4. **Final summary**: average rating, longest comment, unique words, and sorted results

## Sample Results

| Metric | Result |
|---|---|
| Total feedback entries | 13 (10 sample + 3 user-entered) |
| Average rating | 3.62 |
| Feedbacks containing "good" | 4 |
| Feedbacks containing "poor" | 2 |
| Feedbacks containing "excellent" | 1 |
| Longest comment | "poor response and poor handling of issue" |

## Concepts Practiced

- Dictionaries and lists (including appending to lists inside a dictionary)
- `while` loops and nested loops
- String methods: `replace()`, `split()`, `join()`, `lower()`
- Sets for unique values
- Functions with parameters and return values
- `zip()`, `sorted()`, `enumerate()`, `max()`, `sum()`, `len()`

## Getting Started

### Requirements

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Run the project

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

# 2. Install Jupyter (if needed)
pip install notebook

# 3. Launch the notebook
jupyter notebook Python_Project.ipynb
```

Run the cells from top to bottom. When prompted, enter how many feedbacks you want to add, then each name, comment, and rating (1 to 5).

## Repository Structure

```
.
├── Python_Project.ipynb   # Main notebook with all code and outputs
└── README.md
```
