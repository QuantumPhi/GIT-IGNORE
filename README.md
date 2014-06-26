GitignoreAlias
==========
A BASH script used to alias [zachlatta's Gitignorer](https://github.com/zachlatta/gitignorer) into git, allowing for quick
gitignoring of files.

UNIX
----
1. Put the script in your bin
2. Execute ```chmod +x /PATH/TO/BIN/git-ignore```

_WARNING:_

I do not personally own a Mac, so I do not know how this script
will behave in Mac OS. Please open issues or pull requests on
bugs that are found.

```
Usage:
    ignore [OPTIONS]
Options:
    [NO OPTIONS] - Print this help menu
    list - List available templates
    empty - Create empty gitignore
    <TEMPLATE> - Create .gitignore template
    <FILE> - Ignore local file
```

Windows
-------
_Coming soon!_

Licensed under the [MIT License](LICENSE)
