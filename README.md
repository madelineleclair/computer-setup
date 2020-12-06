# Computer setup guide
A repository for setting up any new Mac computer with all the stuff you need to get up and running.

## Install editor

Pick your favorite editor and install it. I use [atom](https://atom.io/). If you use atom, make sure to install the atom shell commands by opening Atom, selecting Atom at the top, and then click `Install Shell Commands`. This will allow you to use the `atom .` command from the terminal. After installing the shell commands, if you have trouble running the `atom` when atom is not running (ex after you just start your computer), you can make an alias for the command, such as `alias atom = 'open -a "Atom"'`

## Install your terminal

Pick your favorite terminal and install it. I use [iTerm2](https://iterm2.com/)

## Install aliases

Aliases make your life so much easier. To install, make a `.zshrc` with `touch ~/.zshrc` for zsh terminals. If your using bash, use `touch ~/.bash_profile`. Open your `.zshrc` or your `.bash_profile` and add the aliases from [my aliases repo](https://github.com/madelineleclair/my_aliases/blob/master/aliases.txt).

## SSH for Github

This allows you to not supply your username and personal access token when you want to connect to Github. To setup SSH, follow the steps from Github: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/connecting-to-github-with-ssh

## Configure Git

When making commits, you want to have the correct name and email set. Once a commit is made, the email and name cannot be changed. For more information, check out the [Git documentation](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

1. Check to see if you have the correct name configured for git
`git config user.name`
2. Check to see if you have the correct email configured for git
`git config user.email`
3. If your username is incorrect, set it
`git config --global user.name "Sally Sue"`
4. If your email is incorrect, set it
`git config --global user.email sallysuee@example.com`

After reconfiguring your name and email, you can verify it by rerunning steps 1 and 2.

## Software installation

Install the following software:

1. [Homebrew](https://brew.sh/): This is a package manager
2. [NVM](https://github.com/nvm-sh/nvm): This is for managing your node versions across multiple apps. I use the curl command for installation. Before executing the command, make sure `~/.zshrc` exists if you use a zsh terminal or `~/.bash_profile` exists if you use a bash terminal. [This article](https://www.codementor.io/@mercurial/how-to-install-node-js-on-macos-sierra-mphz41ekk) also contains good information about installing NVM.
3. [Yarn](https://classic.yarnpkg.com/en/docs/install/#mac-stable): Yarn is another package manager for Javascript dependencies. Once you have Homebrew setup, install it using Homebrew. 
4. [Rbenv](https://github.com/rbenv/rbenv): Rbenv makes it easy to upgrade your ruby version and manage ruby versions across apps.
5. [Postgres](https://wiki.postgresql.org/wiki/Homebrew): PostgresSQL is RDMS. You can install it directly from the website or follow the link to install using Homebrew. Homebrew doesn't give you the GUI like the PostgresSQL website, but it does make it easier to upgrade to a newer version.
