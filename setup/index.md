---
layout: page
title: Testing Setup
root: ..
---

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
    $ python swc-installation-test-2.py git bash jupyter pandas matplotlib
    check Git (git)...			pass
    check Bourne Again Shell (bash)...	pass
    check Jupyter (jupyter)...		pass
    check Pandas (pandas)...		pass
    check Matplotlib (matplotlib)...	pass
    ...
    Successes:

    Git (git) 2.20.1
    Bourne Again Shell (bash) 4.4.23
    Jupyter (jupyter) unknown
    Pandas (pandas) 0.23.4
    Matplotlib (matplotlib) 3.0.2
    ...
    ~~~

    If you see something like:

    ~~~
    $ python swc-installation-test-2.py
    check Bourne Again Shell (bash)...  fail
    ...
    ~~~

    follow the suggestions to try and install any missing software.  For
    additional troubleshooting information, you can use the `--verbose`
    option:

    ~~~
    $ python swc-installation-test-2.py bash --verbose
    check Bourne Again Shell (bash)...  fail
    ...
    ==================
    System information
    ==================
    os.name            : posix
    ...
    ~~~
