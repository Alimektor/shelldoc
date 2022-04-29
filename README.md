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

Use the following template for commenting your bash functions:

```bash
# Public: Short description
#
# [Optional] Long description.
#
# `$1` - The first argument.
# `$2` - The second argument.
# `$3` - The third argument.
# 
# **Examples**
#
#   example_code_with_3_spaces_intend
#
# **Returns**
#
# `0` - If success.
# `1` - If fail.
function func() {}
```

Use the following template for commenting your bash variables:

```bash
# Public: Short description.
#
# Export in environment.
export SHELLDOC="/home/test/shelldoc"
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
