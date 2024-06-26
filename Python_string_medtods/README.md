# Python String Methods #

This document provides an overview of Python's string methods, complete with examples to illustrate their usage.

## Table of Contents.

1.  [capitalize()](#1-capitalize())
2.  [casefold()](#casefold())
3.  [center()](#center())
4.  [count()](#count())
5.  [encode()](#encode())
6.  [endswith()](#endswith())
7.  [expandtabs()](#expandtabs())
8.  [find()](#find())
9.  [format()](#format())
10. [format_map()](#format_map())
11. [index()](#index())
12. [isalnum()](#isalnum())
13. [isalpha()](#isalpha())
14. [isascii()](#isascii())
15. [isdecimal()](#isdecimal())
16. [isdigit()](#isdigit())
17. [isidentifier()](#isidentifier())
18. [islower()](#islower())
19. [isnumeric()](#isnumeric())
20. [isprintable()](#isprintable())
21. [isspace()](#isspace())
22. [istitle()](#istitle())
23. [isupper()](#isupper())
24. [join()](#join())
25. [ljust()](#ljust())
26. [lower()](#lower())
27. [lstrip()](#lstrip())
28. [maketrans()](#maketrans())
29. [partition()](#partition())
30. [replace()](#replace())
31. [rfind()](#rfind())
32. [rindex()](#rindex())
33. [rjust()](#rjust())
34. [rpartition()](#rpartition())
35. [rsplit()](#rsplit())
36. [rstrip()](#rstrip())
37. [split()](#split())
38. [splitlines()](#splitlines())
39. [startswith()](#startswith())
40. [strip()](#strip())
41. [swapcase()](#swapcase())
42. [title()](#title())
43. [translate()](#translate())
44. [upper()](#upper())
45. [zfill()](#zfill())
46. [removeprefix()](#removeprefix())
47. [removesuffix()](#removesuffix())


 ## capitalize()
Description: Converts the first character to uppercase and the rest to lowercase.

```Python

text = "hello WORLD"
print(text.capitalize())  # Output: "Hello world"

```


## casefold()
Description: Converts the string to lowercase in a more aggressive manner than lower(), suitable for case-insensitive comparisons.

```python
Copy code
text = "HELLO WORLD"
print(text.casefold())  # Output: "hello world"

```
## center()
Description: Centers the string in a field of specified width, padding it with a specified character (default is space).

```python
Copy code
text = "hello"
print(text.center(10, '*'))  # Output: "**hello***"
```

## count()
Description: Counts the non-overlapping occurrences of a substring within the string.

```python
Copy code
text = "banana"
print(text.count("a"))  # Output: 3
```
## encode()

 Description: Encodes the string using the specified encoding.

```python
Copy code
text = "hello"
encoded_text = text.encode()
print(encoded_text)  # Output: b'hello'
```

## endswith()
Description: Checks if the string ends with the specified suffix.

```python
Copy code
text = "python.py"
print(text.endswith(".py"))  # Output: True
```
## expandtabs()
Description: Expands tabs in the string to multiple spaces. The default tab size is 8.

```python
Copy code
text = "Hello\tWorld"
print(text.expandtabs(4))  # Output: "Hello   World"
```
## find()
Description: Returns the lowest index in the string where the substring is found. Returns -1 if not found.

```python
Copy code
text = "hello world"
print(text.find("lo"))  # Output: 3
print(text.find("z"))   # Output: -1
```
## format()
Description: Formats the string using the specified arguments.

```python
Copy code
template = "Hello, {}!"
print(template.format("Alice"))  # Output: "Hello, Alice!"
```
## format_map()
Description: Similar to str.format(), but takes a single dictionary argument for replacement fields.


```python
Copy code
template = "Hello, {name}!"
print(template.format_map({"name": "Alice"}))  # Output: "Hello, Alice!"

```
## index()
Description: Similar to find(), but raises a ValueError if the substring is not found.


```python
Copy code
text = "hello world"
print(text.index("lo"))  # Output: 3
# print(text.index("z"))  # Raises ValueError

```
## isalnum()
Description: Checks if all characters in the string are alphanumeric.

```python
Copy code
text = "Hello123"
print(text.isalnum())  # Output: True

text = "Hello 123"
print(text.isalnum())  # Output: False (space is not alphanumeric)
```
## isalpha()
Description: Checks if all characters in the string are alphabetic.

python
Copy code
text = "Hello"
print(text.isalpha())  # Output: True

text = "Hello123"
print(text.isalpha())  # Output: False (contains digits)
isascii()
Description: Checks if all characters in the string are ASCII.

python
Copy code
text = "Hello"
print(text.isascii())  # Output: True

text = "你好"
print(text.isascii())  # Output: False (contains non-ASCII characters)
isdecimal()
Description: Checks if all characters in the string are decimal characters.

python
Copy code
text = "12345"
print(text.isdecimal())  # Output: True

text = "12345.67"
print(text.isdecimal())  # Output: False (contains a dot)
isdigit()
Description: Checks if all characters in the string are digits.

python
Copy code
text = "12345"
print(text.isdigit())  # Output: True

text = "12345.67"
print(text.isdigit())  # Output: False (contains a dot)
isidentifier()
Description: Checks if the string is a valid identifier according to Python's rules.

python
Copy code
text = "hello_world"
print(text.isidentifier())  # Output: True

text = "123hello"
print(text.isidentifier())  # Output: False (starts with a digit)
islower()
Description: Checks if all characters in the string are lowercase.

python
Copy code
text = "hello"
print(text.islower())  # Output: True

text = "Hello"
print(text.islower())  # Output: False (contains an uppercase letter)
isnumeric()
Description: Checks if all characters in the string are numeric.

python
Copy code
text = "12345"
print(text.isnumeric())  # Output: True

text = "Ⅷ"  # Roman numeral for 8
print(text.isnumeric())  # Output: True
isprintable()
Description: Checks if all characters in the string are printable.

python
Copy code
text = "Hello, World!"
print(text.isprintable())  # Output: True

text = "Hello\nWorld"
print(text.isprintable())  # Output: False (contains a newline)
isspace()
Description: Checks if all characters in the string are whitespace.

python
Copy code
text = "   "
print(text.isspace())  # Output: True

text = "Hello"
print(text.isspace())  # Output: False
istitle()
Description: Checks if the string is titlecased.

python
Copy code
text = "Hello World"
print(text.istitle())  # Output: True

text = "Hello world"
print(text.istitle())  # Output: False (second word is not capitalized)
isupper()
Description: Checks if all characters in the string are uppercase.

python
Copy code
text = "HELLO"
print(text.isupper())  # Output: True

text = "Hello"
print(text.isupper())  # Output: False (contains a lowercase letter)
join()
Description: Joins elements of an iterable into a single string, with the string acting as a separator.

python
Copy code
words = ["Hello", "world"]
print(" ".join(words))  # Output: "Hello world"

numbers = ["1", "2", "3"]
print("-".join(numbers))  # Output: "1-2-3"
ljust()
Description: Left-justifies the string in a field of the specified width, padding it with a specified character (default is space).

python
Copy code
text = "hello"
print(text.ljust(10, '*'))  # Output: "hello*****"
lower()
Description: Converts all characters in the string to lowercase.

python
Copy code
text = "HELLO WORLD"
print(text.lower())  # Output: "hello world"
lstrip()
Description: Removes leading characters (space is the default) from the string.

python
Copy code
text = "   hello   "
print(text.lstrip())  # Output: "hello   "

text = "---hello---"
print(text.lstrip('-'))  # Output: "hello---"
maketrans()
Description: Returns a translation table used by the translate() method.

python
Copy code
intab = "aeiou"
outtab = "12345"
trantab = str.maketrans(intab, outtab)

text = "hello world"
print(text.translate(trantab))  # Output: "h2ll4 w4rld"
partition()
Description: Splits the string into a tuple (head, sep, tail) at the first occurrence of sep.

python
Copy code
text = "hello world"
print(text.partition(" "))  # Output: ('hello', ' ', 'world')
replace()
Description: Replaces occurrences of a substring with another substring.

python
Copy code
text = "hello world"
print(text.replace("world", "Python"))  # Output: "hello Python"
rfind()
Description: Returns the highest index in the string where the substring is found. Returns -1 if not found.

python
Copy code
text = "hello world"
print(text.rfind("lo"))  # Output: 3
print(text.rfind("z"))   # Output: -1
rindex()
Description: Similar to rfind(), but raises a ValueError if the substring is not found.

python
Copy code
text = "hello world"
print(text.rindex("lo"))  # Output: 3
# print(text.rindex("z"))  # Raises ValueError
rjust()
Description: Right-justifies the string in a field of the specified width, padding it with a specified character (default is space).

python
Copy code
text = "hello"
print(text.rjust(10, '-'))  # Output: "-----hello"
rpartition()
Description: Splits the string into a tuple (head, sep, tail) at the last occurrence of sep.

python
Copy code
text = "hello world"
print(text.rpartition(" "))  # Output: ('hello', ' ', 'world')
rsplit()
Description: Splits the string into a list using the specified separator, starting from the end.

python
Copy code
text = "apple,banana,cherry"
print(text.rsplit(','))  # Output: ['apple', 'banana', 'cherry']
rstrip()
Description: Removes trailing characters (space is the default) from the string.

python
Copy code
text = "   hello   "
print(text.rstrip())  # Output: "   hello"

text = "---hello---"
print(text.rstrip('-'))  # Output: "---hello"
split()
Description: Splits the string into a list using the specified separator.

python
Copy code
text = "apple,banana,cherry"
print(text.split(','))  # Output: ['apple', 'banana', 'cherry']

text = "The quick brown fox"
print(text.split())  # Output: ['The', 'quick', 'brown', 'fox']
splitlines()
Description: Splits the string at line breaks into a list.

python
Copy code
text = "hello\nworld"
print(text.splitlines())  # Output: ['hello', 'world']

text = "hello\nworld\n"
print(text.splitlines(True))  # Output: ['hello\n', 'world\n']
startswith()
Description: Checks if the string starts with the specified prefix.

python
Copy code
text = "hello world"
print(text.startswith("hello"))  # Output: True

print(text.startswith("world"))  # Output: False
strip()
Description: Removes leading and trailing characters (space is the default) from the string.

python
Copy code
text = "   hello world   "
print(text.strip())  # Output: "hello world"

text = "---hello---"
print(text.strip('-'))  # Output: "hello"
swapcase()
Description: Swaps case of all characters in the string.

python
Copy code
text = "Hello World"
print(text.swapcase())  # Output: "hELLO wORLD"
title()
Description: Converts the first character of each word to uppercase and the rest to lowercase.

python
Copy code
text = "hello world"
print(text.title())  # Output: "Hello World"
translate()
Description: Translates the string using a translation table created by str.maketrans().

python
Copy code
intab = "aeiou"
outtab = "12345"
trantab = str.maketrans(intab, outtab)

text = "hello world"
print(text.translate(trantab))  # Output: "h2ll4 w4rld"
upper()
Description: Converts all characters in the string to uppercase.

python
Copy code
text = "hello world"
print(text.upper())  # Output: "HELLO WORLD"
zfill()
Description: Pads the string with zeros on the left to fill a specified width.

python
Copy code
text = "42"
print(text.zfill(5))  # Output: "00042"
removeprefix()
Description: Removes the specified prefix from the string if it exists.

python
Copy code
text = "HelloWorld"
print(text.removeprefix("Hello"))  # Output: "World"
removesuffix()
Description: Removes the specified suffix from the string if it exists.

python
Copy code
text = "HelloWorld"
print(text.removesuffix("World"))  # Output: "Hello"
