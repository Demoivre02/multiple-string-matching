# String Matching Algorithms

This repository contains Python implementations of various string matching algorithms, including Aho-Corasick and Commentz-Walter algorithms.

## Algorithms

1. **Aho-Corasick**: A string searching algorithm that finds all occurrences of a set of keywords in a given text.

2. **Commentz-Walter**: An improvement over the Aho-Corasick algorithm for multiple string matching, offering efficient matching of reversed keywords.

3. **Fast Practical Multiple String Matching**: Combines Aho-Corasick with a DAWG (Directed Acyclic Word Graph) for fast and practical multiple string matching.

## Usage

To use these algorithms, you can import the respective classes and create instances with your set of keywords. Then, use the provided methods for searching in a text.

Example:

```python
# Aho-Corasick Example
keywords = ["apple", "orange", "banana"]
acm = AhoCorasick(keywords)
text = "I like apples and bananas."
matches = list(aho_corasick_search(text, len(text), acm))
print(matches)
