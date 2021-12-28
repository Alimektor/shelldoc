# shelldoc docs
A simple utility for creating [Tomdoc](http://tomdoc.org/) style documentation for bash script.


Table of Contents
=================

   * [usage()](#usage)
   * [run_shelldoc()](#run_shelldoc)


`usage()`
---------

Public: usage example

Print usage example of shelldoc

* `$0` - script name

**Examples**

    usage

**Returns**

nothing, but print usage text


`run_shelldoc()`
----------------

Public: Create a markdown doc for shell script.

* `--in` - input script file
* `--out` - output doc file
* `--header` - header of the doc file
* `--desc` - description of the script in doc file
* `--access` - [optional] access for script. Added at the beginning of the function comment

**Examples**

    shelldoc --in input.sh --out out.md --header "My awesome script" --desc "The great description"

**Returns**

* `0` - if success
* `1` - exit if fail
