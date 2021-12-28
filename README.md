Shelldoc
========

A simple utility for creating [Tomdoc](http://tomdoc.org/) style documentation for bash script.

Installation
------------

```bash
git clone --recurse-submodules https://github.com/Alimektor/shelldoc.git
```

Usage
-----

### Example Doc ###

Shelldoc Usage in [Tomdoc style](shelldoc.md#run_shelldoc)

### Help message ###

```bash
./shelldoc -h
```

### Quick Start ###

Use the following template for commenting your bash scripts:

```bash
# Public: Short description
#
# [Optional] Long description
#
# `$1` - the first argument
# `$2` - the second argument
# `$3` - the third argument
# 
# **Examples**
#
#   example_code_with_3_spaces_intend
#
# **Returns**
#
# `0` - if success
# `1` - if fail
function func() {}
```

Examples
--------

```bash
./shelldoc --in shelldoc --out shelldoc.md --header "shelldoc docs" --desc "A simple utility for creating [Tomdoc](http://tomdoc.org/) style documentation for bash script." --access "Public"
```

* [input file](shelldoc)
* [output file](shelldoc.md)

Limitations
-----------

The `github-markdown-toc` module requires a connection to the GitHub API to create the table of contents.

License
-------

[MIT](LICENSE.md)
