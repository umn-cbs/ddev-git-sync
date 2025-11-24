[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/umn-cbs/ddev-git-sync/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/umn-cbs/ddev-git-sync/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/umn-cbs/ddev-git-sync)](https://github.com/umn-cbs/ddev-git-sync/commits)
[![release](https://img.shields.io/github/v/release/umn-cbs/ddev-git-sync)](https://github.com/umn-cbs/ddev-git-sync/releases/latest)

# DDEV Git Sync

## Overview

This add-on integrates Git Sync into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get umn-cbs/ddev-git-sync
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Git Sync |
| `ddev logs -s git-sync` | Check Git Sync logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.git-sync --git-sync-docker-image="ddev/ddev-utilities:latest"
ddev add-on get umn-cbs/ddev-git-sync
ddev restart
```

Make sure to commit the `.ddev/.env.git-sync` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `GIT_SYNC_DOCKER_IMAGE` | `--git-sync-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@umn-cbs](https://github.com/umn-cbs)**
