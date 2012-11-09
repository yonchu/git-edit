# git-edit

`git-edit` is git subcommand to edit modified and untracked files with zsh completion.

## Installation

Clone `git-edit` from github.

```shell
$ git clone git://github.com/yonchu/git-edit.git
```

Put `git-edit` file to PATH directory (like ~/bin).

```shell
$ cd git-edit
$ cp git-edit ~/bin
$ chmod +x ~/bin/git-edit
```

If you uses zsh, put `_git-edit` file to zsh functions directory (like /usr/share/zsh/site-functions/ or /usr/local/share/zsh/site-functions/).

```shell
$ cp _git-edit /usr/local/share/zsh/site-functions/
$ exec zsh
```

## Usage

```shell
$ git edit [commit] [file ...]
```
- No argument : Edit all modified and untracked files.

- [commit] : Specify commit object.(e.g. HEAD, hash value)

- [file ...] : Specify files which want to Edit.(Also can specify wildcard like `git edit *.txt`.


If you uses zsh, you can use completion.

```shell
$ git edit <TAB>
Modified Files
xxxx.txt    yyyy.sh    zzzz.c

$ git edit HEAD <TAB>
Modified Files(HEAD=62c91ef1f56d89b3328fa4aeae4bb52b579ad679)
aaaa.txt    bbbb.sh    cccc.c
```
Go in a git repository and test it!

**Enjoy your git and zsh life!!**


See also
---------------

* [よんちゅBlog](http://yonchu.hatenablog.com/)
