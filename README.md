# leincalc
LaTeX package for typesetting calculus documents

## Installation

Download or clone the repository.  Within the repository's directory, execute:

    $ l3build install --full

This _should_ install the package in a place that your TeX installation can
find it and also that you can write to.  The particular place depends on your
operating system and TeX distributions.  The author uses MacOS and TeX-live.  
Package and class files are installed in `~/Library/texmf/tex/latex`.

The `--full` command line option also installs documentation.  In the author's
system, it goes into `~/Library/texmf/doc/latex`.

If your `l3build` does not support the `--full` option, you can try to upgrade
it.  For instance, in TeX-live, the command

    $ sudo tlmgr update l3build

will do it.  Or you can omit the option, and execute these commands:

    $ l3build install
    $ cp -r build/distrib/tds/doc `kpsewhich --var-value TEXMFHOME`/doc

## Documentation

If you installed the documentation in the right place, you can read it with:

    $ texdoc leincalc

If you did not install documentation at all, you can do:

    $ l3build doc
    $ open build/doc/leincalc.pdf

