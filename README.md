# fish-python

Better fish configuration for python

## What you get?

- Better `python` completions
- Better `ipython` completions
- Better `jupyter` completions
- Cool new functions
- venv handling

## venv

Python 3 added the venv module, which replaces all the other ways that the
community created to make Python virtual environments.

But, if you have ever used virtualenv and virtualenvwrapper, there are some
convenience commands that make working with Python virtual environments easier.

This plugin gives you a `workon` command for activating a venv, as well as the
`mkvenv` command to make Python virtual environments.

Virtual environments are stored in $VENV_HOME, which defaults to
`~/.local/share/venvs`

### Sample usage

```fish
# make a venv at ~/.local/share/venvs/playground
mkvenv playground

# mkvenv is just a wrapper around "python3 -m venv", so pass other arguments
# to it at will.
mkvenv --without-pip --copies --prompt 'wanna play?' another_playground

# activate a virtual environment
workon playground

# do your work here...
# ???

# when done, deactivate
deactivate
```

## Install

Fisher:

```shell
# fisher installation
fisher add https://github.com/mattmc3/fish-python
```

OMF:

```shell
# oh-my-fish installation
omf install https://github.com/mattmc3/fish-python
```
