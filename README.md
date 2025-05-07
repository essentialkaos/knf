<p align="center"><a href="#readme"><img src=".github/images/card.svg"/></a></p>

<p align="center">
  <a href="https://kaos.sh/w/knf/ci"><img src="https://kaos.sh/w/knf/ci.svg" alt="GitHub Actions CI Status" /></a>
  <a href="https://kaos.sh/w/knf/codeql"><img src="https://kaos.sh/w/knf/codeql.svg" alt="GitHub Actions CodeQL Status" /></a>
  <a href="#license"><img src=".github/images/license.svg"/></a>
</p>

<p align="center"><a href="#installation">Installation</a> • <a href="#command-line-completion">Command-line completion</a> • <a href="#man-documentation">Man documentation</a> • <a href="#usage">Usage</a> • <a href="#ci-status">CI Status</a> • <a href="#contributing">Contributing</a> • <a href="#license">License</a></p>

<br/>

`knf` is a simple utility for reading values from [KNF files](https://kaos.sh/knf-spec).

### Installation

#### From source

To build the `knf` from scratch, make sure you have a working [Go 1.23+](https://github.com/essentialkaos/.github/blob/master/GO-VERSION-SUPPORT.md) workspace (_[instructions](https://go.dev/doc/install)_), then:

```
go install github.com/essentialkaos/knf@latest
```

#### Prebuilt binaries

You can download prebuilt binaries for Linux and macOS from [EK Apps Repository](https://apps.kaos.st/knf/latest):

```bash
bash <(curl -fsSL https://apps.kaos.st/get) knf
```

### Command-line completion

You can generate completion for `bash`, `zsh` or `fish` shell.

Bash:
```bash
sudo knf --completion=bash 1> /etc/bash_completion.d/knf
```

ZSH:
```bash
sudo knf --completion=zsh 1> /usr/share/zsh/site-functions/knf
```

Fish:
```bash
sudo knf --completion=fish 1> /usr/share/fish/vendor_completions.d/knf.fish
```

### Man documentation

You can generate man page using next command:

```bash
knf --generate-man | sudo gzip > /usr/share/man/man1/knf.1.gz
```

### Usage

<img src=".github/images/usage.svg"/>

### CI Status

| Branch | Status |
|--------|----------|
| `master` | [![CI](https://kaos.sh/w/knf/ci.svg?branch=master)](https://kaos.sh/w/knf/ci?query=branch:master) |
| `develop` | [![CI](https://kaos.sh/w/knf/ci.svg?branch=develop)](https://kaos.sh/w/knf/ci?query=branch:develop) |

### Contributing

Before contributing to this project please read our [Contributing Guidelines](https://github.com/essentialkaos/.github/blob/master/CONTRIBUTING.md).

### License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://kaos.dev"><img src="https://raw.githubusercontent.com/essentialkaos/.github/refs/heads/master/images/ekgh.svg"/></a></p>
