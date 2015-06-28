file-auto-renamer
http://spenibus.net
https://github.com/spenibus/file-auto-renamer-php-cli
https://gitlab.com/spenibus/file-auto-renamer-php-cli

Renames multiple files in multiple directories using callbacks.

Files in "./config":
   directories.txt
      Contains a list of directories, one per line, in which to look for files
      to be renamed.
   filter-%name%.txt
      A filter file containing a regular expression to match files and a
      callback to rename them.
      %name% is a user-chosen string to help identify and organize filter files.
      Multiple filter files can be used.

Filter file format:
   -  First line is a regular expression used to match files to be renamed.
   -  The rest of the file is a php function serving as callback to the regular
      expression to provide a new filename.

Sample configuration is available in "./config-example".