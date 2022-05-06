==============
setuptools-npm
==============

Plugin for setuptools to run npm commands.

-----
Usage
-----

This command provides `npm_install` and `npm_run` commands.

Run `python setup.py npm_install --help` or `python setup.py npm_run --help`
for available options.

`npm_not_skipped` is a helper function that can be used as predicate for
distutils subcommand. It evaluates to `True` if env variable `SKIP_NPM`
is not defined. This variable is exclusive to this helper function and
is not evaluated in `npm_install` and `npm_run` commands themselves.
