# regex
A compiled list of regex for learning


####One or more times
---
Use the + operator

example

```
/l(ol)+/
```

matches lolololol

####Character Set and Ranges
---
Use the square braces [x] for character set
Use the - for a range, e.g 1-5 or a-z

example
```
/[a-z]/
```
represents a small case letter inside the alphabet
matches 'a', 'b'

####Case Insensitive
---
Use the 'i' modifier to make the regex case insensitive

example
```
/[a-z]/i
```

matches 'a', 'B', 'C'

####White space
---
Use \s to represent white space

example
```
/\s/
```

matches space, tab, newlines

####Word Metacharacter
---
\w is the same as [a-zA-Z0-9];

example
```
/\w/
```

matches 'a', 'F', '3'

###wildcard
---
Use the dot . to represent anything except for a new line

example

```
/./
```

matches any one character

###Optional, matches zero or one times
---
Use the question mark ? to represent something that is matched zero or one times

example
```
/ba?/
```
matches 'ba', 'b'

###Groups
---
Use groups to group stuff together ();

example
```
/test(ing|ed)/
```
matches 'testing', 'tested'

##Anchors
###Start with
---
use the ^ to signify starting with

example
```
/^test/
```
matches 'test', 'tester', 'testing'

###End At
---
Use the $ to signify end at

example
```
/hook$/
```

matches 'prehook', 'posthook'

##Word Boundaries
Use the \b to define word boundaries

example
```
/\bwhat\b/
```

matches 'dont know whats wrong'

##Not
Use the caret ^ for not, must be in square brackets

example
```
/[^a]/
```

matches 'b', 'c'

##Number
Use the \d for numbers, same as [0-9]

example
```
/\d/
```

matches '1', '5'

##capitalized Metacharacter
Stands for the opposite \D is anything that is not a number

example
```
/\D/
```

matches 'a', 'c', ','

##Intervals
use {min,max} to match a interval number of items

```
/a{2,4}/
```

matches 'aa', 'aaa', 'aaaa'
