# Learning git
## Topics

Will be revised in this repository:
 - Git flow
 - Commits Signatures
 - Branches configurations
 - PR / PR templates
 - Code reviews
 - VSCode plugin
 - Code owners
 - "SemVer" ~Semantic Versioning
 - Convetional commits

## Git flow
 Git flow is used to keep our branches organized, bugfixes, feature, main, development and such as tags and more.

 There is a git [extension](https://github.com/petervanderdoes/gitflow-avh) that could help

 [Git flow workflow from BitBucket](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

## Commits signatures
 Use GPG to sign your commits, a safe way to know who really commited
 - Install GPG
 - Generate key with `gpg --full-generate-key`
 - Get your GPG key's ID with `gpg -K --keyid-form LONG`
 - Print and copy your GPG key with `gpg --armor --export <YOUR KEYID>`
 - Add the copied GPG key at Github
 - Add GPG `tty` to your bash or zsh adding into the settings file: `export GPG_TTY=$(tty)`
 - Setup your git to use this GPG to sign your commits with `git config [--global,--system,--local,--worktree] user.signingkey <YOUR KEYID>`
 - Config git to sign on commit with `git config [--global,--system,--local,--worktree] commit.gpgsign true`
 - Config git to sign on tag creation with `git config [--global,--system,--local,--worktree] tag.gpgsign true`

Additional information found:
 - [SSH access using a GPG key for authentication](https://opensource.com/article/19/4/gpg-subkeys-ssh)
 - [About gpg-agent](https://www.systutorials.com/docs/linux/man/1-gpg-agent/)

 ## Pull requests

 [VSCode extension](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)

 ## Semantic Versioning

 [Semantic Versioning documentation](https://semver.org/)

## Conventional Commits

[Convetional Commits documentation](https://www.conventionalcommits.org/en/v1.0.0/)
[VSCode extension](https://marketplace.visualstudio.com/items?itemName=vivaxy.vscode-conventional-commits)

## commitlint

[Documentation](https://commitlint.js.org/#/guides-local-setup)

## Commitizen

[Documentation](https://commitizen-tools.github.io/commitizen/)

# CI
## commitsar

[Documentatios](https://commitsar.aevea.ee/)