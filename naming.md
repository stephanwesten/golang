# Introduction
This is an opioniated guide on naming conventions in Go. For an explanation see the [Background](#background) section.



# General Convention
The convention in Go is to use MixedCaps or mixedCaps rather than underscores to write multiword names. (CamelCase)
Snakecase, using underscores, is hardly used. Afaik only for test file names with the postfix 'test'.

# Package names
See the [General Convention](#general-convention) section.


The package name and the functions should be such that you get a readable contract like `bytes.Encode`.

References
- See https://golang.org/doc/effective_go.html#package-names

# Variable names
See the [General Convention](#general-convention) section.

# Types
See the [General Convention](#general-convention) section.

# File names
See the [General Convention](#general-convention) section.

# Background
There are several kind of programmers, e.g. math oriented, text oriented, fysics oriented. I belong to the textual variant and as such I prefer clear and explicit names. A type name like Record is for me a no-go :smirk:. I prefer explicit names like BackupRecord.

As such I disagree with some of the conventions in the Go world. For example I disagree with the Go naming statement "A helpful doc comment can often be more valuable than an extra long name."
The comment is only written in one place, not in the places where the object (variable, function) is used. Sometimes you will forget to jump to the declaration and read the comment and make false assumptions. Of course I value comments *a lot*. But comments should be there to explain the deeper meaning, lessons learned and, if needed, the intents in the long run: how should the code evolve. Of course this will lead to long comments. This is a concious choice, the trade-off is that information should be as close to the code as possible and not in a far away feature/issue tracking system. I see comments as a way to exchange information between developers in a team - perhaps remote. 

Other examples where I disagree:
- using one letter variables is a terrible practice.
- prefering user above userName. I want to know straight away whether i'm dealing with a struct or a string.
