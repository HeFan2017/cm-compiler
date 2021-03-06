llvm-profdata - work with profile data
======================================

SYNOPSIS
--------

:program:`llvm-profdata` [-output=output] file1 file2

DESCRIPTION
-----------

The experimental :program:`llvm-profdata` tool reads two profile data files
generated by PGO instrumentation and generates a file with merged data.

The profile data format itself is currently textual.

OPTIONS
-------

.. option:: -output=output

 This option selects the output filename.  If not specified, output is to
 stdout.

EXIT STATUS
-----------

:program:`llvm-profdata` returns 1 if it cannot read input files or there is a
mismatch between their data.
