# git-ignore-template
Generate multilingual .gitignore files from github/gitignore

## Installation
Copy `git-ignore-template` to a directory on your `PATH` and make it executable:

```sh
cp git-ignore-template /usr/local/bin/git-ignore-template
```

Git will automatically recognize it as a subcommand, so you can invoke it as
`git ignore-template`.

## Usage
```sh
git ignore-template <template> [<template> ...]
git ignore-template --append <template> [<template> ...]
```

Fetches the specified templates from
[github/gitignore](https://github.com/github/gitignore) and writes them to
`.gitignore` in the current directory. Use `--append` to add to an existing
`.gitignore` instead of overwriting it.

### Examples
```sh
git ignore-template Go Python
git ignore-template C "C++" Node
git ignore-template --append Java Maven
```

Template names are case-sensitive and correspond to filenames in the
[github/gitignore](https://github.com/github/gitignore) repository (e.g. `Go`,
`C++`, `Maven`).

## Contributing
Bug reports and patches are welcome. Please open a pull request.

## License
GNU General Public License v2.0
