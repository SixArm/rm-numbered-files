# Remove numbered files

This script removes numbered files and related kinds of archive files.

Contents:

* [Introduction](#introduction)
* [Which files?](#which-files)
* [Related](#related)
* [Compatibility notes](#compatibility-notes)
* [Tracking](#tracking)


## Introduction

Syntax:

    $ rm-numbered-files [dir]

Example to do the current directory:

    $ rm-numbered-files

Example to do a specific directory:

    $ rm-numbered-files /foo/goo


## Which files?

This deletes files with names that end in a separator then number:

  * foo.1, foo-2, foo_3, etc.

The file name separator can be a period, dash, or underscore.


## Related

These scripts are for related purposes:

  * [rm-compressed-files](https://github.com/SixArm/rm-compressed-files)

  * [rm-dated-files](https://github.com/SixArm/rm-dated-files)

  * [rm-numbered-files](https://github.com/SixArm/rm-numbered-files)

  * [rm-rotated-files](https://github.com/SixArm/rm-rotated-files)


## Compatibility notes

We prefer to be more compatible rather than system-specific.

  * To delete files, we prefer `-exec rm` vs. `-delete`.
    The former is more compatible, the latter is faster.

  * To regex match, we prefer patterns to be basic vs. extended.
    The former is more compatible, the latter is more modern.

  * We prefer POSIX code vs. shell-specific code.


## Tracking

  * Command: rm-numbered-files
  * Website: http://sixarm.com/rm-numbered-files
  * Cloning: https://github.com/sixarm/rm-numbered-files
  * Version: 4.0.0
  * Created: 2013-12-09
  * Updated: 2019-01-01
  * License: GPL
  * Contact: Joel Parker Henderson (joel@joelparkerhenderson.com)
  * Tracker: 7f2b1f4ed3481e5912a9f4e5f5a92a34
