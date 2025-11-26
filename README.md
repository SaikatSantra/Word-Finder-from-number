# Phone Keypad Word Matcher

This project converts phone keypad digits into possible matching words from a given dictionary.  
Example: **1-800-FLOWERS → 1-800-3569377**, where **FLOWERS → 3569377** using the phone keypad mapping.

## Task Overview

Given:

- Phone number: **3662277**
- Dictionary: ["foo", "flowers", "bar", "foobar", "emo", "cap", "car", "cat", "far", "ra"]


Find all dictionary words whose keypad digit representation appears as a contiguous substring of the phone number.

## Keypad Mapping
`const singleTap = {
  a:"2", b:"2", c:"2",
  d:"3", e:"3", f:"3",
  g:"4", h:"4", i:"4",
  j:"5", k:"5", l:"5",
  m:"6", n:"6", o:"6",
  p:"7", q:"7", r:"7", s:"7",
  t:"8", u:"8", v:"8",
  w:"9", x:"9", y:"9", z:"9",
  " ": "0"
};`

## Output

| Word   | Number | Match |
|--------|--------|--------|
| foo    | 366    | ✔ |
| emo    | 366    | ✔ |
| bar    | 227    | ✔ |
| cap    | 227    | ✔ |
| car    | 227    | ✔ |
| foobar | 366227 | ✔ |


