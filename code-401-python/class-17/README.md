# Python Regular Expression

## Regular Expressions, often shortened as regex, : are a sequence of characters used to check whether a pattern exists in a given text (string) or not.

## Regular expressions are useful in search and replace operations. The typical use case is to look for a sub-string that matches a pattern and replace it with something else. Most APIs using regular expressions allow you to reference capture groups from the search pattern in the replacement string.

## Regular Expressions in Python
### In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

### import re


## Grouping in Regular Expressions
### The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual.

## Summary Table
![regex expression](https://miro.medium.com/max/1400/1*veWrrw0abBahg31ipuxArQ.png)


## Function Provided by 're'
## The re library in Python provides several functions to make your tasks easier. You have already seen some of them, such as the re.search(), re.match().

- compile(pattern, flags=0)
- search(pattern, string, flags=0)
- match(pattern, string, flags=0)
- findall(pattern, string, flags=0) 
- finditer(string, [position, end_position])
- sub(pattern, repl, string, count=0, flags=0)
- subn(pattern, repl, string, count=0)
- split(string, [maxsplit = 0])
- start() - Returns the starting index of the match.
- end() - Returns the index where the match ends.
- span() - Return a tuple containing the (start, end) positions of the match.


# shutil — High-level File Operations
## The shutil module includes high-level file operations such as copying and archiving.

## Copying Files
### copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file

## Copying File Metadata
### By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

## Working With Directory Trees
### shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

## Finding Files
### The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

## Archives
### Python’s standard library includes many modules for managing archive files such as tarfile and zipfile. There are also several higher-level functions for creating and extracting archives in shutil. get_archive_formats() returns a sequence of names and descriptions for formats supported on the current system.

