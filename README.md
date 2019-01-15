# git-simple

git-simple is a command-line tool that provides shortcuts for many common git workflows. [Version 0.0]

## Usage

First, make sure you have Git installed. Then, download this repo and place the `gitsp` file in a directory on your machine. For ease of use, either:

1. Place `gitsp` in a directory then add that directory to `$PATH`, or
2. Place `gitsp` in a directory that is already in `$PATH`

And you're ready to rock and roll! It may be necessary to change permissions for the file with either `chmod +x gitsp` or `sudo chmod +x gitsp`.

## Commands

In general, call git-simple with `gitsp`, then follow that with the desired command.

#### init

`gitsp init <remote_url>`

Initializes a git repository in the current folder and also connects it to the specified remote URL.

#### send

`gitsp send <files> <commit_msg> [<branch]`

Combines the `add`, `commit` and `push` git commands into one. Specify which files to push as well as the commit message, and give an optional branch to push to. Pushes to master by default.

#### pull

`gitsp pull [<branch>]`

Stashes changes then pulls from the remote repository, and then applies the stashed changes back to show merge conflicts, if any. Pulls from the specified branch, or from master by default.

#### create

`gitsp create <branch>`

Creates a new local branch with the specified name.

#### switch

`gitsp switch <branch>`

Switches to the specified local branch.

#### delete

`gitsp delete <branch>`

Deletes the specified local branch.

#### user

`gitsp user <username> <email>`

Configures user credentials for commits.

#### info

`gitsp info`

Shows some information about the current repository, including username, email, remote URL, and local branches.

#### help

`gitsp help`

Shows a list of all available `gitsp` commands.

#### version

`gitsp version` or  `gitsp -v`

Shows the installed `gitsp` version.

## Future Improvements/Additions:

- Dedicated merge command
- Rebase command
- Commit unstage command
- Fetch command
