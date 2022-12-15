# cloneall
Clone all github repos of an org

## Overview
This is a script to clone all Github repos of an org with one command.

## Installation
Download the `cloneall` script and place it in an executabe path, like `/usr/local/bin/`.

## Pre-requisites
This script needs a few tools to be in place for it to work:

1. curl
2. jq
3. git
4. SSH auth keys [configured at Github](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

## Usage
First, it may be a good idea to create a directory for <org> and change into it:

```
$ mkdir <org>
$ cd <org>
```

Then, invoke the scipt by passing the org as the parameter:

```
$ cloneall <org>
```

## Notes
This tool may work well for a handful of repos. If you have a whole lof of repos in your org, you'll have to consider the implications of Github's rate limiting. YMMV.
