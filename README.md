# Computing Group Rank with Limited Nondeterminism #

This file was last updated on 19 December 2014.

Elsevier article class
----------------------

The document `grouprank.tex` uses a modified `elsarticle` document class. The
class was modified as described [here][0] in order to allow usage with
BibLaTeX. The modified class file can be found in `elsarticlenonatbib`. It is
distributed under the LaTeX Project Public License; for more information, see
the header comments in that file.

[0]: https://hopstat.wordpress.com/2014/10/09/biblatex-with-elsarticle/

Downloading
-----------

The markup is available from GitHub.

    git clone git@github.com:jfinkels/grouprank

A somewhat recent version of the compiled document should be available at
https://cs-people.bu.edu/jeffreyf/static/pdf/grouprank.pdf, but I can't
guarantee that that will always be up to date, since I compile and upload it
manually.

Compilation dependencies
------------------------

Compilation requires `pdflatex`, `biber`, and the following LaTeX packages:

* `amsmath`
* `amsthm`
* `babel`
* `biblatex`
* `complexity`
* `csquotes`
* `hyperref`
* `thmtools`
* `tikz`

To install these packages on Ubuntu 11.04 through 14.04:

    sudo apt-get install texlive-base texlive-latex-base texlive-latex-extra \
      texlive-science texlive-pictures biber

Compiling
---------

To compile the document, run

    pdflatex grouprank
    biber grouprank
    pdflatex grouprank

The output is `grouprank.pdf`, and can be viewed with any PDF reader.

Copyright
---------

Copyright 2014 Jeffrey Finkelstein.

Both the LaTeX markup and the content of this article are made available under
the terms of the Creative Commons Attribution-ShareAlike 4.0 International
License, https://creativecommons.org/licenses/by-sa/4.0/.

Contact
-------

Jeffrey Finkelstein <jeffreyf@bu.edu>
