# Coverage.py Badge

A small script to generate coverage badges using Coverage.py.

The badge template has been taken from [shields.io](http://shields.io/),
therefore it should look mostly good. (The spec is a bit stricter on the
margins, but I can't easily do text width calculations in Python so the margins
might not always be 4px.)


## Usage

Change to a directory where coverage data (in the `.coverage` file) is
available. If you don't have this file yet, you need to run coverage first.

Then you can either return the badge SVG to stdout:

    $ coverage-badge

...or write it to a file:

    $ coverage-badge -o coverage.svg

The full usage:

    usage: coverage_badge [-h] [-o FILEPATH] [-q]

    Generate coverage badges for Coverage.py.

    optional arguments:
      -h, --help   show this help message and exit
      -o FILEPATH  Save the file to the specified path.
      -q           Don't output any non-error messages.


## License

MIT License.
