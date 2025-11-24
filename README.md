[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![last commit](https://img.shields.io/github/last-commit/umn-cbs/ddev-git-sync)](https://github.com/umn-cbs/ddev-git-sync/commits)
[![release](https://img.shields.io/github/v/release/umn-cbs/ddev-git-sync)](https://github.com/umn-cbs/ddev-git-sync/releases/latest)

# DDEV Git Sync

## Overview

This add-on synchronizes the host's global git config into the web container. A post-start hook is included to ensure configs are pulled in every time the web container is started.

## Installation

```bash
ddev add-on get umn-cbs/ddev-git-sync
ddev restart
```

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev git-sync` | Command synchronizes the host's global git config into the web container |
