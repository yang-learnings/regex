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
