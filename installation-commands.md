**install autocomplete for git**

`curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash`

once command finished, add code below to ~/.bash_profile

```
if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi
```
Install homebrew

Install nvm for managing node version

https://www.codementor.io/@mercurial/how-to-install-node-js-on-macos-sierra-mphz41ekk

Install yarn using homebrew. (this make it easier to upgrade in the future)
https://classic.yarnpkg.com/en/docs/install/#mac-stable

Use rbenv for managing ruby versions
