# shelldoc docs

A simple utility for creating [Tomdoc](http://tomdoc.org/) style documentation for bash script.


Table of Contents
=================

   * [usage()](#usage)
   * [run_shelldoc()](#run_shelldoc)


`usage()`
---------

Public: Usage example

Print usage example of shelldoc.

* `$0` - Script name.

**Examples**

    usage

**Returns**

Nothing, but print usage text.


`run_shelldoc()`
----------------

Public: Create a markdown doc for shell script

* `--in` - Input script file.
* `--out` - Output doc file.
* `--header` - Header of the doc file.
* `--desc` - Description of the script in doc file.
* `--access` - [optional] Access for script. Added at the beginning of the function comment.

**Examples**

    shelldoc --in input.sh --out out.md --header "My awesome script" --desc "The great description"

**Returns**

* `0` - (exit code) If success.
* `1` - (exit code) If fail.
