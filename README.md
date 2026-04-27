# Nepali NLP Parser

This is a simple rule-based NLP parser for Nepali text.
It can split sentences, tag parts of speech, and generate a basic dependency structure.

The goal of this project is to show how NLP can be implemented without using heavy libraries or machine learning.

---

## What it does

* Breaks text into tokens
* Assigns POS tags using a small dictionary + rules
* Finds simple relationships like subject, object, and root

---

## How to run

```bash
python nepaliparser.py
```

Then enter a Nepali sentence when prompted.

Example:

```
राम किताब पढ्छ
```

---

## Example output

```
Tokens: ['राम', 'किताब', 'पढ्छ']

POS:
राम -> PROPN  
किताब -> NOUN  
पढ्छ -> VERB  

Dependencies:
राम -> nsubj  
किताब -> obj  
पढ्छ -> ROOT  
```

---

## Notes

* No external libraries are used
* Everything is based on simple rules and patterns
* Accuracy depends on the dictionary and heuristics

---

## Future ideas

* Improve word coverage
* Add name/entity detection
* Make parsing rules a bit smarter

---

This was built mainly for learning and experimentation with basic NLP concepts.
