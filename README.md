# Simple Git Guide

![If that doesn't fix it, git.txt contains the phone number of a friend of mine who understands git. Just wait through a few minutes of 'It's really pretty simple, just think of branches as...' and eventually you'll learn the commands that will fix everything.](http://imgs.xkcd.com/comics/git.png)


## Git Directory Setup

Required: [Git](https://git-scm.com/downloads)

Clone the repository, for example:

```sh
$ git clone https://path/to/git/repository.git
```

Navigate to the newly created directory:

```sh
$ cd <project name>
```

Set your `user.name` and `user.email`:

```sh
$ git config user.name "John Doe"
$ git config user.email "john.doe@example.com"
```

To check if your information was saved correctly, use:

```sh
$ git config --list
```

Now you can make your additions/changes to files


## Commit

Track all your files:

```sh
$ git add .
```

Alternatively, you can track an individual file with:

```sh
$ git add <filename>
```

To check the status of your files, use:

```sh
$ git status
```

Commit your changes. Add `-m` to set a custom commit message:

```sh
$ git commit -m "example commit message"
```

Continue your coding process and perform another commit, or push your changes to the server.

## Push

`origin` is the name of the *remote server*. `master` is the name of the target *branch*.

These names were automatically set up by `git clone`.

Simply:

```sh
$ git push origin master
```

## Pull

When your collaborators push their commits to the server, you should pull them to keep your local files up to date.

```sh
$ git pull
```

Under normal circumstances there should be no *merge conflicts*.

## Merge Conflicts

*Conflicts* happen when multiple changes are made to the same line of code.

You have to merge these *conflicts* manually by editing your files shown by git.

After you are done. Finish the merge by performing a commit:

```sh
$ git add <filename>
$ git commit
```

## The Next Step

For further information, refer to these guides:
* https://rogerdudler.github.io/git-guide/
* https://git-scm.com/doc
* http://lmgtfy.com/?q=git

## Other (GUI) Tools

* [Source Tree](https://www.sourcetreeapp.com/) is a full-featured git client with a friendly interface.
* [Ungit](https://github.com/FredrikNoren/ungit) is an opensource web-based git GUI.
* [GitKraken](http://www.gitkraken.com/) is a cross-platform git client under active development.
