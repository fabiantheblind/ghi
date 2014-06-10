# ghi
GitHub Interface - a minimal command line tool

## Description

Simple command line tool created to automate the repetative GitHub operations I perform regularly.

## Installation

### Developer (you want to contribute)
If you'd like to contribute to the repo:
  1. clone down the repo

    ```sh
    git clone git@github.com:phillipalexander/ghi.git
    ```

  1. cd to the root directory of the project

    ```sh
    cd ./ghi
    ```

  1. use [npm-link](https://www.npmjs.org/doc/cli/npm-link.html) to create a local link to the github repo so that you can develop on it more effectively

    ```sh
    npm link
    ```

  1. start hacking!

### Basic (you just want it to work)

If you're not insterested in contributing right now, just use npm to install ghi:

```
$ npm install -g ghi
```

## Configuration

To use the ghi tool, you must configure the config.json file in the root directory. To do so, run any of the commands below and follow the instructions.

## Commands

### rc (Repo Create)

```sh
Usage: rc <orgname/reponame>
Description: Repo Create: Create a repo on GitHub
Example: ghi rc macroscope/blog
Options:

  -h, --help     output usage information
  -V, --version  output the version number
```

### rd (Repo Destroy)

```sh
Usage: rd <orgname/reponame>
Description: Repo Destroy: Destroy a repo on GitHub
Example: ghi rd macroscope/blog
Options:

  -h, --help     output usage information
  -V, --version  output the version number
```

### rha (Repo Hook Add)

```sh
Usage: rha <orgname/reponame>
Description: Repo Hook Add: Add webhook defined in config.json to a repo
Example: ghi rha macroscope/blog
Options:

  -h, --help     output usage information
  -V, --version  output the version number
```

### rta (Repo Team Add)

```sh
Usage: rta <orgname/reponame>
Description: Repo Team Add: Add all teams listed in config.json to an existing repo
Example: ghi rta macroscope/blog
Options:

  -h, --help     output usage information
  -V, --version  output the version number
```

### rga (Repo Get All)

```sh
Usage: rga <orgname>
Description: Repo Get All: Get the first 100 repos associated with an Org
Example: ghi rga macroscope
Options:

  -h, --help     output usage information
  -V, --version  output the version number
```

### tga (Team Get All)

```sh
Usage: tga <orgname>
Description: Team Get All: Get the first 100 teams associated with an Org
Example: ghi tga macroscope
Options:

  -h, --help     output usage information
  -V, --version  output the version number
```

### tua (Team User Add)

```sh
Usage: tua [options]
Description: Team User Add: Add a GitHub user to an existing team
Example: ghi tua -o "macroscope" -t "awesome force" -u "jasper"
Options:

  -h, --help             output usage information
  -o, --org <orgname>    GitHub Org
  -t, --team <teamname>  GitHub Team
  -u, --user <username>  GitHub Username
```

For additional usage instructions, run

```
ghi --help
```

## License

Copyright (c) 2014 Phillip Alexander

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
