# Schematic
[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)

## Introduction

SCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, data ingress ecosystem, that is meant to streamline the process of dataset annotation, metadata validation and submission to an asset store (e.g., [Synapse](https://www.synapse.org/)) for various data contributors.

## Installation Requirements and Pre-requisites

* Python 3.7.1 or higher

Note: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.

* Clone of the [ncihtan/data-models](https://github.com/ncihtan/data-models) repository

```
git clone https://github.com/ncihtan/data-models.git
```

Configure the [config.yml](https://github.com/ncihtan/data-models/blob/main-add-files/config.yml) file in the `data-models` directory appropriately. All paths in `config.yml` are specified relative to the `config.yml` file.

## Installing

Create and activate a virtual environment within which you can install the package:

```
python -m venv .venv
source .venv/bin/activate
```

Install and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):

```
python -m pip install schematicpy
```

## Command Line Client Usage

### Initialization

```
schematic init --config ~/path/to/config.yml    # initialize mode of authentication
```

### Manifest

```
schematic manifest --config ~/path/to/config.yml get    # generate manifest based on data type
```

```
schematic manifest --config ~/path/to/config.yml validate   # validate manifest
```

### Model

```
schematic model --config ~/path/to/config.yml submit    # validate and submit manifest
```

## Contributing

Interested in contributing? Awesome! We follow the typical [GitHub workflow](https://guides.github.com/introduction/flow/) of forking a repo, creating a branch, and opening pull requests. For more information on how you can add or propose a change, visit our [contributing guide](CONTRIBUTION.md). To start contributing to the package, you can refer to the [Getting Started](CONTRIBUTION.md#getting-started) section in our [contributing guide](CONTRIBUTION.md).

## Contributors

Active contributors and maintainers:

- [Milen Nikolov](https://github.com/milen-sage)
- [Sujay Patil](https://github.com/sujaypatil96)
- [Bruno Grande](https://github.com/BrunoGrandePhD)
- [Xengie Doan](https://github.com/xdoan)
