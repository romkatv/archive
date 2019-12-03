Archive
=======

Create, list, and extract archives.

Commands
---------

  - `archive` creates an archive based on the provided archive name.
  - `lsarchive` lists the contents of one or more archives.
  - `unarchive` extracts the contents of one or more archives.

Supported Formats
-----------------

The following archive formats are supported when the required utilities are
installed:

  - *.tar.gz*, *.tgz* require `tar` (optionally `pigz`).
  - *.tar.bz2*, *.tbz* require `tar` (optionally `pbzip2`).
  - *.tar.xz*, *.txz* require `tar` with *xz* support.
  - *.tar.lzma*, *.tlz* require `tar` with *lzma* support.
  - *.tar* requires `tar`.
  - *.gz* requires `gunzip`.
  - *.bz2* requires `bunzip2`.
  - *.xz* requires `unxz`.
  - *.lzma* requires `unlzma`.
  - *.Z* requires `uncompress`.
  - *.zip*, *.jar* requires `unzip`.
  - *.rar* requires `rar` (needed for `archive` support), `unrar` or `lsar` and `unar`.
  - *.7z* requires `7za`.
  - *.deb* requires `ar`, `tar`.

Additionally, if `pigz` and/or `pbzip2` are installed, `archive` will use them
over their traditional counterparts, `gzip` and `bzip2` respectively, to take
full advantage of all available CPU cores for compression.

Provenance
-------

Forked from
[prezto](https://github.com/sorin-ionescu/prezto/tree/2d6205e71404704eecc4f402e5b09d7cbd19bab7).
