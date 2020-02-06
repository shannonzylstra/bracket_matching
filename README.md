[![Run on Repl.it](https://repl.it/badge/github/shannonzylstra/bracket_matching)](https://repl.it/github/shannonzylstra/bracket_matching)

# Challenge: Bracket Matching

Bracket matching is a very common example usage of a stack. Many programming language compilers and interpreters use stacks for parsing language syntax, specifically for detecting when you open a code block and then when that code block is closed. This is called 'bracket matching'

Create a method in Python called `test_brackets` that takes a `string` and determines if all brackets are correctly matching / nested (returns `True` or `False`). This is code could be used as part of a system to detect syntax errors in code.

It should check for the following: `[ ]`,`{ }`,`( )`

### Usage Examples

```python
test_brackets('abc(123)')
#returns true

test_brackets('abc(123')
#returns false -- missing closing bracket

test_brackets('a[bc(123)]')
#returns true

test_brackets('a[bc(12]3)')
#returns false -- inproperly nested

test_brackets('a{b}{c(1[2]3)}')
#returns true

test_brackets('a{b}{c(1}[2]3)')
#returns false -- inproperly nested

test_brackets('()')
#returns true

test_brackets('[]]')
#returns false - no opening bracket to correspond with last character

test_brackets('abc123yay')
#returns true -- no brackets = correctly matched
```
