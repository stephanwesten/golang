This is an opioniated guide on naming conventions in Go.
There are several kind of programmers, e.g. math oriented, text oriented, fysics oriented. I belong to the textual variant.

As such I disagree with some of the conventions in the Go world. I disagree with the Go naming statement "A helpful doc comment can often be more valuable than an extra long name."
The comment is only in one place, not in the places where e.g. the function is used. Also, imo using one letter variables is a terrible practice.

# General
The convention in Go is to use MixedCaps or mixedCaps rather than underscores to write multiword names. (CamelCase)
Snakecase, using underscores, is hardly used. Afaik only for test file names with the postfix 'test'.

# Package names
See https://golang.org/doc/effective_go.html#package-names

the package name and the functions should be such that you get a readable contract like `bytes.Encode`.

# Variable names


# Types


# File names
