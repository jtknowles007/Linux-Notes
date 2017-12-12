# Pandoc

## 12/11/2017

* Pandoc can take a markdown file and combine it with a css file to output fully styled html.  This can be achieved by running the following:

~~~~~
pandoc foo.md -s -c style.css --self-contained -o foo.html
~~~~~

* Pandoc flags used in above example
    + -s (or --standalone) produces output with an appropriate header and footer to create a standalone file of the filetype specified.  Pandoc's default is to produce a document fragment
    + -c links to a css stylesheet.  can pbe used repeatedly to include multiple files
    + --self-contained produces a standalone html file with no external dependencies.  Used to include images, stylesheets, videos, and such
    + -o write output to a file instead of stdout
* Pandoc also supports remote files, so you can replace style.css with a remote css file (https://somewhere.com/style.css)
*
