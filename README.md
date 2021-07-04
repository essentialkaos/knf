<p align="center"><a href="#readme"><img src="https://gh.kaos.st/knf.svg"/></a></p>

<p align="center">
  <a href="https://kaos.sh/w/knf/ci"><img src="https://kaos.sh/w/knf/ci.svg" alt="GitHub Actions CI Status" /></a>
  <a href="https://kaos.sh/r/knf"><img src="https://kaos.sh/r/knf.svg" alt="GoReportCard" /></a>
  <a href="https://kaos.sh/b/knf"><img src="https://kaos.sh/b/4373cae8-963f-40f0-a45c-ff32b5a785fa.svg" alt="Codebeat badge" /></a>
  <a href="https://kaos.sh/w/knf/codeql"><img src="https://kaos.sh/w/knf/codeql.svg" alt="GitHub Actions CodeQL Status" /></a>
  <a href="#license"><img src="https://gh.kaos.st/apache2.svg"></a>
</p>

<p align="center"><a href="#installation">Installation</a> • <a href="#command-line-completion">Command-line completion</a> • <a href="#man-documentation">Man documentation</a> • <a href="#usage">Usage</a> • <a href="#build-status">Build Status</a> • <a href="#contributing">Contributing</a> • <a href="#license">License</a></p>

<br/>

`knf` is a simple utility for reading values from KNF files.

### Installation

#### From source

To build the `knf` from scratch, make sure you have a working Go 1.15+ workspace (_[instructions](https://golang.org/doc/install)_), then:

```
go install github.com/essentialkaos/knf
```

#### Prebuilt binaries

You can download prebuilt binaries for Linux and OS X from [EK Apps Repository](https://apps.kaos.st/knf/latest):

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

```
Usage: knf {options} knf-file property

Options

  --exist, -E        Checks if given param is exist
  --no-color, -nc    Disable colors in output
  --help, -h         Show this help message
  --version, -v      Show version

Examples

  knf file.knf server:ip
  Read server:ip param value

  knf -E file.knf server:ip
  Checks if server:ip param is exist in KNF file

```

### Build Status

| Branch | Status |
|--------|----------|
| `master` | [![CI](https://kaos.sh/w/knf/ci.svg?branch=master)](https://kaos.sh/w/knf/ci?query=branch:master) |
| `develop` | [![CI](https://kaos.sh/w/knf/ci.svg?branch=develop)](https://kaos.sh/w/knf/ci?query=branch:develop) |

### Contributing

Before contributing to this project please read our [Contributing Guidelines](https://github.com/essentialkaos/contributing-guidelines#contributing-guidelines).

### License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
