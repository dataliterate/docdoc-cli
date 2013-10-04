# docdoc

is a tool and work principle designed by precious.

It helps people to document their design process.

----------

# docdoc-cli

The docdoc command line interface.

Install this globally and you'll have access to the `docdoc` command anywhere on
your system.

**Note:** The job of the docdoc command is to load and run the version of docdoc
you have installed locally to your documentation, irrespective of its version.

This architectur is heavily inspired by the
[grunt-cli](https://github.com/gruntjs/grunt-cli). 

Each docdoc documentation has a package.json and a custom Docdocfile.js where
plugins are loaded and configured. Also the docdoc-generator code should be part
of a documentation. Everything is kept in a folder named `_docdoc`. This is by
convention.

Use the docdoc-cli that should be installed as global module.
The cli code looks for the _docdoc folder and than executes the generator.

This architecture avoids version conflicts between generator and plugins, as each documentation may upgrade its generator and plugins whenever needed.

## Installation

Not yet.
