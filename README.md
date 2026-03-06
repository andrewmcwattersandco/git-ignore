# git-ignore
Generate multilingual .gitignore files from github/gitignore

## Installation
Copy `git-ignore` to a directory on your `PATH` and make it executable:

```sh
cp git-ignore /usr/local/bin/git-ignore
```

Git will automatically recognize it as a subcommand, so you can invoke it as `git ignore`.

## Usage
```sh
git ignore <lang> [<lang> ...]
git ignore --append <lang> [<lang> ...]
```

Fetches the specified templates from [github/gitignore](https://github.com/github/gitignore) and writes them to `.gitignore` in the current directory. Use `--append` to add to an existing `.gitignore` instead of overwriting it.

### Examples
```sh
git ignore Go Python
git ignore C "C++" Node
git ignore --append Java Maven
```

Template names are case-sensitive and correspond to filenames in the [github/gitignore](https://github.com/github/gitignore) repository (e.g. `Go`, `C++`, `Maven`).

## Contributing
Bug reports and patches are welcome. Please send them to the project mailing list or open a pull request on GitHub.

## License
GNU General Public License v2.0
