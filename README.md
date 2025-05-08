[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/tyler36/ddev-site-metrics-github/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/tyler36/ddev-site-metrics-github/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/tyler36/ddev-site-metrics-github)](https://github.com/tyler36/ddev-site-metrics-github/commits)
[![release](https://img.shields.io/github/v/release/tyler36/ddev-site-metrics-github)](https://github.com/tyler36/ddev-site-metrics-github/releases/latest)

# DDEV Site Metrics Github

## Overview

This add-on integrates Site Metrics Github into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get tyler36/ddev-site-metrics-github
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Site Metrics Github |
| `ddev logs -s site-metrics-github` | Check Site Metrics Github logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.site-metrics-github --site-metrics-github-docker-image="busybox:stable"
ddev add-on get tyler36/ddev-site-metrics-github
ddev restart
```

Make sure to commit the `.ddev/.env.site-metrics-github` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `SITE_METRICS_GITHUB_DOCKER_IMAGE` | `--site-metrics-github-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@tyler36](https://github.com/tyler36)**
