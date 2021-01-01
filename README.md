# Here is my personnal settings to code

## Some lib

- [Terminal Markdown Viewer](https://github.com/axiros/terminal_markdown_viewer)
- [Color ls](https://github.com/athityakumar/colorls)
- [Spaceship](https://github.com/denysdovhan/spaceship-prompt)

```shell
autoload -U promptinit; promptinit
prompt restore
source $(dirname $(gem which colorls))/tab_complete.sh
```

## Some scripts
*Scripts to place in your .bashrc or .zshrc*

### Display list of commit's hash of your current branch and copy to clipboard

```shell
function get_hash() {
    git log --oneline | fzf | cut -f 1 -d" " | xclip -selection clipboard
}
```

### Get the name of current branch in clipboard

```shell
function gitname() {
    git rev-parse --abbrev-ref HEAD | xclip -selection clipboard
}

```

## Some software settings

[Vs Code](./vscode/README.md)