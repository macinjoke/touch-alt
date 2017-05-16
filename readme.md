# [![touch-alt](media/logo.png)](https://github.com/akameco/touch-alt) [![Build Status](https://travis-ci.org/akameco/touch-alt.svg?branch=master)](https://travis-ci.org/akameco/touch-alt)

> Create from a template instead of a new file


## Install

```
$ npm install --global touch-alt
```

## Demo

![demo](./media/demo.gif)


## Usage

```
$ touch-alt --help

  Create from a template instead of a new file

  Usage
  $ touch-alt <source>
  $ touch-alt --add <source>

  Options
  -a, --add         Create new template file
  -o, --overwrite   Overwrite by template

  Example
  $ touch-alt .editorconfig
```

## Example

### Add new template file

```
$ cat .editorconfig
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true
$ touch-alt --add .editorconfig
```

### Usage

```
# Use touch
$ touch .editorconfig
$ cat .editorconfig

$ rm .editorconfig

# Use touch-alt
$ touch-alt .editorconfig
$ cat .editorconfig
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true
```


## Tip
Add `alias touch=touch-alt` to your .zshrc/.bashrc to reduce typing & create file easily.


## License

MIT © [akameco](http://akameco.github.io)
