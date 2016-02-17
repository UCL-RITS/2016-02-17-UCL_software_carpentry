---
layout: page
title: Testing Setup
root: ..
---
# Test your setup

This directory contains scripts for testing your machine to make sure
you have the software you'll need for your workshop installed.  To use
these scripts:

1.  Download [swc-installation-test-1.py](swc-installation-test-1.py).

2.  Run it from the shell:

    ~~~
    $ python swc-installation-test-1.py
    Passed
    ~~~

3.  Download [swc-installation-test-2.py](swc-installation-test-2.py).

4.  Run it from the shell:

    ~~~
    $ python swc-installation-test-2.py
    check virtual-shell...  pass
    ...
    Successes:

    virtual-shell Bourne Again Shell (bash) 4.2.37
    ...
    ~~~

    If you see something like:

    ~~~
    $ python swc-installation-test-2.py
    check virtual-shell...  fail
    ...
    check for command line shell (virtual-shell) failed:
      command line shell (virtual-shell) requires at least one of the following dependencies
      For instructions on installing an up-to-date version, see
      http://software-carpentry.org/setup/
      causes:
      check for Bourne Again Shell (bash) failed:
        could not find 'bash' executable for Bourne Again Shell (bash)
        For instructions on installing an up-to-date version, see
        http://software-carpentry.org/setup/
    ...
    ~~~

    follow the suggestions to try and install any missing software.  For
    additional troubleshooting information, you can use the `--verbose`
    option:

    ~~~
    $ python swc-installation-test-2.py --verbose
    check virtual-shell...  fail
    ...
    ==================
    System information
    ==================
    os.name            : posix
    ...
    ~~~

# Get ready for Python

1.  Make a new folder in your Desktop called `python-novice-inflammation`.

1.  Download
    [`python-novice-inflammation-data.zip`](http://swcarpentry.github.io/python-novice-inflammation/python-novice-inflammation-data.zip)
    and move the file to this folder.

1.  If it's not unzipped yet, double-click on it to unzip it. You should end up
    with a new folder called `data`.

1.  From the shell:

    ~~~
    $ cd && cd Desktop/python-novice-inflammation/data
    $ jupyter notebook
    ~~~
