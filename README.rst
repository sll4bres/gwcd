GWCD: Wherigo files (.gwc) decompiler
=====================================

This script is a simple Wherigo files (.gwc) decompiler. As we known how a .gwc
is formatted [1], we can read the file in binary mode, extracting data along the
reading.

This script can be used to :

- retrieve data related to the Wherigo (included the completion code),
- extract the compiled Lua file (describing the scenario of the cartridge),
- extract media files.

Usage
-----

::

    $ python gwcd.py [OPTIONS] <gwc file>

Options are::

    -h, --help       show this help message and exit
    --output OUTPUT  Output directory where gwcd will store extracted data
    --lua            Extract compiled lua file
    --completion     Show the completion code
    --media          Extract media files
    --verbose, -v    Show all data related to the cartridge
    --all            Do everything

Licence
-------
BSD Licence. See LICENCE file.

Sources
-------
[1] https://github.com/WFoundation/WF.Compiler
