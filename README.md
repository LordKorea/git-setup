# git-setup

A script providing a `git setup` command which automates (my) github and gitlab
repository creation workflow.

## Installation

Put the script into your `$PATH`, e.g. `~/.local/bin`.

For full functionality, you need a personal access token for both GitHub and
GitLab. The location of the token files is hardcoded to be in the `.ssh`
directory in the user's home directory. These default paths can be easily
changed by editing the script, however.

GitHub access token file: `~/.ssh/github_token`

GitLab access token file: `~/.ssh/gitlab_token`

## Usage

Invoke the script via `~$ git setup`. An interactive dialogue will request all
further information.

## Features

* Creates a GitHub repo
* Creates a GitLab repo
* Optionally creates a discord webhook for both repos

## Future Work

* Automatically set up push mirroring from GitLab -> GitHub (currently not
supported by GitLab API)
