# Remove numbered files

This script removes numbered files and related kinds of archive files.

TThis deletes files with names that end in a separator then number:

  * foo.1, foo-2, foo_3, etc.

Syntax:

    rm-numbered-files [dir]

Example to do the current directory:

    rm-numbered-files

Example to do a specific directory:

    rm-numbered-files /foo/goo

The file name separator can be a period, dash, or underscore.


## Compatibility notes

We prefer to be more compatible rather than system-specific.

  * To delete files, we prefer `-exec rm` vs. `-delete`.
    The former is more compatible, the latter is faster.

  * To regex match, we prefer patterns to be basic vs. extended.
    The former is more compatible, the latter is more modern.

  * We prefer POSIX code vs. shell-specific code.


## Tracking

  * Command: rm-numbered-files
  * Version: 3.0.0
  * Created: 2013-12-09
  * Updated: 2017-08-29
  * License: GPL
  * Contact: Joel Parker Henderson (joel@joelparkerhenderson.com)
