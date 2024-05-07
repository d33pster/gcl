# gcl -> the new git clone

gcl is the new command for cloning your repositories (public and private). Rising from the rust (pun intended), its fast and reliable.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Private Repositories](#private-repositories)

## Installation

For installation simply run

```bash
cargo install gcl
```

## Usage

For help Text run,

```console
$ gcl help
gcl v1.0
Help Text

syntax: $ gcl [options] username repo <optional-destination-dir> [flags]

  | [Options]
  | help -> show help and exit.
  | version -> show version and exit.

  | [Flags]
  | --priv -> for private repos, add this flag.
```

`NOTE:` flags can be placed anywhere in the command. Be sure to follow this sequence -> username, repo, path.

Example usage:

```bash
gcl d33pster gcl home/
# this will clone into home/gcl/
```

```bash
gcl d33pster warlock --priv home/
# this will clone into home/warlock/
```

## Private Repositories

For private repositories, You will be needing a GitHub Token (classic).

Steps to get a classic token:

- Click on you profile pic, go to settings.
- Go to Developer Settings.
- Click on Personal Acess Token, select Tokens (Classic).
- Click on generate new Token and select Tokens (Classic).

When running `gcl` for the first time with `--priv` flag, it will ask for a tokens classic. Copy and paste it. This is one time only.
