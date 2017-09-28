# nlp
NLTK code snippets


**Example 1**
```python
"""
This sentence does not end with punctuation
This sensence does.
"""
```
- Q: Are they one or two sentences when using the sentence tokenizer?
- A: They are treated as one sentence because whitespace doesn't matter for a tokenizer

**Example 2**
```python
"""
This sentence does not end with punctuation

This sensence does.
"""
```
- Q: Are they one or two sentences when using the sentence tokenizer?
- A: They are treated as one sentence because whitespace doesn't matter for a tokenizer. That includes newline ```\n```

This code provides a solution if you want to make double newline```\n\n | \n \n``` a marker of a new sentence
