# Word Wrap

You write a class called Wrapper, that has a single static function named wrap that takes two arguments: a string, and a column number. The function returns the string, but with line breaks inserted at just the right places to make sure that no line is longer than the column number. You try to break lines at word boundaries.

Like a word processor, break the line by replacing the last space in a line with a newline.

## Extra

Add hyphenation. Create a hardcoded list with known words with syllables, for example:
```
dic‧tion‧ary
en‧cy‧clo‧pe‧dia
vo‧cab‧u‧lary
```

Make long words that are present in the list wrap on the given syllables where applicable, for example:
```
Look it up in the dic-
tionary.
```

Mind that the hyphen takes up one space as well.
