Curriculum Short Specializations Average: 99.98% Markdown to HTML Python HTML By: Guillaume, CTO at Holberton School Weight: 1 Project will start May 2, 2023 6:00 AM, must end by May 8, 2023 6:00 AM Checker will be released at May 3, 2023 6:00 PM An auto review will be launched at the deadline Description Markdown is awesome! All your README.md are made in Markdown, but do you know how GitHub are rendering them?

It’s time to code a Markdown to HTML!

Requirements All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7 or higher) The first line of all your files should be exactly #!/usr/bin/python3 A README.md file, at the root of the folder of the project, is mandatory Your code should use the PEP 8 style (version 1.7.*) All your files must be executable All your modules should be documented: python3 -c 'print(import("my_module").doc)' Your code should not be executed when imported (by using if name == "main":) Tasks 0. Start a script #advanced Write a script markdown2html.py that takes an argument 2 strings:

First argument is the name of the Markdown file Second argument is the output file name Requirements:

If the number of arguments is less than 2: print in STDERR Usage: ./markdown2html.py README.md README.html and exit 1 If the Markdown file doesn’t exist: print in STDER Missing and exit 1 Otherwise, print nothing and exit 0 guillaume@vagrant:/$ ./markdown2html.py Usage: ./markdown2html.py README.md README.html guillaume@vagrant:/$ echo $? 1 guillaume@vagrant:/$ guillaume@vagrant:/$ ./markdown2html.py README.md README.html Missing README.md guillaume@vagrant:/$ echo $? 1 guillaume@vagrant:/$ guillaume@vagrant:/$ echo "Test" > README.md guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:~/$ Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py

Heading #advanced Improve markdown2html.py by parsing Headings Markdown syntax for generating HTML:
Syntax: (you can assume it will be strictly this syntax)

Markdown HTML generated

Heading level 1
Heading level 1
Heading level 2
Heading level 1
Heading level 3
Heading level 1
Heading level 4
Heading level 1
Heading level 5
Heading level 1
Heading level 6
Heading level 1
guillaume@vagrant:~/$ cat README.md

My title
My title2
My title3
My title4
My title5
guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:/$ cat README.html

My title
My title2
My title3
My title4
My title5
guillaume@vagrant:~/$ Spacing and new lines between HTML tags don’t need to be exactly this one
Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py

Unordered listing #advanced Improve markdown2html.py by parsing Unordered listing syntax for generating HTML:
Syntax: (you can assume it will be strictly this syntax)

Markdown:

Hello
Bye HTML generated:
Hello
Bye
guillaume@vagrant:~/$ cat README.md # My title - Hello - Bye
guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:/$ cat README.html

My title
Hello
Bye
guillaume@vagrant:~/$ Spacing and new lines between HTML tags don’t need to be exactly this one
Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py

Ordered listing #advanced Improve markdown2html.py by parsing Ordered listing syntax for generating HTML:
Syntax: (you can assume it will be strictly this syntax)

Markdown:

Hello
Bye HTML generated:
Hello
Bye
guillaume@vagrant:~/$ cat README.md # My title * Hello * Bye
guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:/$ cat README.html

My title
Hello
Bye
guillaume@vagrant:~/$ Spacing and new lines between HTML tags don’t need to be exactly this one
Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py

Simple text #advanced Improve markdown2html.py by parsing paragraph syntax for generating HTML:
Syntax: (you can assume it will be strictly this syntax)

Markdown:

Hello

I'm a text with 2 lines HTML generated:

Hello

I'm a text
with 2 lines

guillaume@vagrant:~/$ cat README.md # My title - Hello - Bye
Hello

I'm a text with 2 lines

guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:/$ cat README.html

My title
Hello
Bye
Hello

I'm a text
with 2 lines

guillaume@vagrant:~/$ Spacing and new lines between HTML tags don’t need to be exactly this one
Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py

Bold and emphasis text #advanced Improve markdown2html.py by parsing bold syntax for generating HTML:
Syntax: (you can assume it will be strictly this syntax)

Markdown HTML generated Hello Hello Hello Hello guillaume@vagrant:~/$ cat README.md

My title
Hello
Bye
Hello

I'm a text with 2 lines

Or in bold

guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:/$ cat README.html

My title
Hello
Bye
Hello

I'm a text
with 2 lines

Or in bold

guillaume@vagrant:~/$ Spacing and new lines between HTML tags don’t need to be exactly this one
Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py

... but why?? #advanced Improve markdown2html.py by parsing bold syntax for generating HTML:
Syntax: (you can assume it will be strictly this syntax)

Markdown HTML generated description [[Hello]] 8b1a9953c4611296a827abf8c47804d7 convert in MD5 (lowercase) the content ((Hello Chicago)) Hello hiago remove all c (case insensitive) from the content guillaume@vagrant:~/$ cat README.md

My title
Hello
Bye
Hello

I'm a text with 2 lines

((I will live in Caracas))

But it's [[private]]

So cool!

guillaume@vagrant:/$ ./markdown2html.py README.md README.html guillaume@vagrant:/$ cat README.html

My title
Hello
Bye
Hello

I'm a text
with 2 lines

I will live in araas

But it's 2c17c6393771ee3048ae34d6b380c5ec

So cool!

guillaume@vagrant:~/$ Spacing and new lines between HTML tags don’t need to be exactly this one
Repo:

GitHub repository: alx-frontend-for-fun File: markdown2html.py
