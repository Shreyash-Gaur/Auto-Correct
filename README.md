---

# Autocorrect System

This repository contains a Jupyter notebook that implements a simple yet effective auto-correct system. This project demonstrates fundamental concepts in natural language processing (NLP) and string manipulation techniques used in autocorrect systems.

## Table of Contents
- [Overview](#overview)
- [Data Preprocessing](#data-preprocessing)
  - [process_data](#process_data)
  - [get_count](#get_count)
  - [get_probs](#get_probs)
- [String Manipulations](#string-manipulations)
  - [delete_letter](#delete_letter)
  - [switch_letter](#switch_letter)
  - [replace_letter](#replace_letter)
  - [insert_letter](#insert_letter)
- [Combining the Edits](#combining-the-edits)
  - [edit_one_letter](#edit_one_letter)
  - [edit_two_letters](#edit_two_letters)
  - [get_corrections](#get_corrections)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)

## Overview

The autocorrect system aims to correct misspelled words by suggesting the most probable correct spelling. This project involves several key tasks:

- Counting word frequencies in a corpus.
- Calculating word probabilities.
- Performing string manipulations to generate possible corrections.
- Using edit distance to determine the most likely corrections.

## Data Preprocessing

### process_data
Processes raw text data to prepare it for analysis. This function reads the corpus and cleans the data, making it ready for further processing.

### get_count
Counts the frequency of each word in the corpus. This helps in understanding the distribution of words in the text.

### get_probs
Calculates the probability of each word based on its frequency. This probability distribution is used to suggest the most likely corrections.

## String Manipulations

### delete_letter
Generates all possible strings by deleting one letter from the input word.

### switch_letter
Generates all possible strings by switching adjacent letters in the input word.

### replace_letter
Generates all possible strings by replacing each letter in the input word with every other letter.

### insert_letter
Generates all possible strings by inserting a letter at every position in the input word.

## Combining the Edits

### edit_one_letter
Combines the string manipulations to generate all possible words resulting from a single edit (insertion, deletion, replacement, or switch).

### edit_two_letters
Generates all possible words resulting from two edits. This function extends the single-edit manipulations to consider combinations of two edits.

### get_corrections
Suggests possible corrections for a misspelled word by comparing the edit distances and probabilities. It returns a list of the most likely corrections.

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required Python libraries: `numpy`, `pandas`, `collections`

### Installation
Clone the repository:
```bash
git clone https://github.com/Shreyash-Gaur/Auto-Correct.git
cd Auto-Correct
```

Install the required libraries:
```bash
pip install numpy pandas
```

## Usage
Open the Jupyter notebook:
```bash
jupyter notebook Autocorrect.ipynb
```

Run the cells in the notebook to see the implementation of the autocorrect system. Each section includes explanations and examples to help you understand the code.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

---
