# MyTool {Title/Reponame}

> Helps you build things {one-line purpose}

{} = Explanations for this readme..

Maybe here is a small overview of how `MyTool`, should not be longer than 5 lines and you're invited to use emojis 👯.

<!-- TOC depthFrom:2 -->

- [Setup {Install instructions}](#setup-install-instructions)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
- [Usage {Describe how to use the component}](#usage-describe-how-to-use-the-component)
    - [Bootstrap environment](#bootstrap-environment)
    - [Start](#start)
    - [Tests](#tests)
- [Mystuff {you can add individual headings at this point}](#mystuff-you-can-add-individual-headings-at-this-point)
- [License](#license)

<!-- /TOC -->

{Headings defined here are required (unless not implemented) but you're free to add custom headings above `License`}
## Setup {Install instructions}

### Prerequisites

* Python `>=2.6 & < 3`
* GNU compiler
* node `>= 8`

### Installation

{Please make sure you have simple installation instructions or bundle them into a `Makefile`}
```sh
npm install
# or python
make install
```

## Usage {Describe how to use the component}

### Bootstrap environment

`MyTool` needs the following supporting components to run on your system:

* MySQL 2.9.3 at `2701`
* Redis 3 at `3102`

To start them in a docker environment you can use the following command:

{Make sure that this command is also not overly long}

```sh
make env-up
```

### Start
There are two ways to start `MyTool`

```sh
npm run
# or python
make run / python tool.py
```

or you can use `docker run openmined/mytool` to start a prepared docker container with the latest release.

### Tests

```sh
make test
# or nodeJS
npm test
```

You can run codestyle checks with

```sh
make lint
# or nodeJS
npm lint
```

## Mystuff {you can add individual headings at this point}

I want to thank my mom and dad for giving me a computer when I was 8 years old.

## License

[Apache-2.0](LICENSE) by OpenMined contributors {Valid SPDX License name}