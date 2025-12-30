# Golang Text Wrapper with Indent

[![GoDoc](https://pkg.go.dev/badge/github.com/bassosimone/textwrapper)](https://pkg.go.dev/github.com/bassosimone/textwrapper) [![Build Status](https://github.com/bassosimone/textwrapper/actions/workflows/go.yml/badge.svg)](https://github.com/bassosimone/textwrapper/actions) [![codecov](https://codecov.io/gh/bassosimone/textwrapper/branch/main/graph/badge.svg)](https://codecov.io/gh/bassosimone/textwrapper)

The `textwrapper` Go package contains code to wrap and indent text.

For example:

```Go
import "github.com/bassosimone/textwrapper"

const (
	indent = "    "
	width = 72
)
output := textwrapper.Do(paragraph, width, indent)
```

The above example wraps paragraph with the given four spaces
indent such that lines are `<=` 72 chars.

## Installation

To add this package as a dependency to your module:

```sh
go get github.com/bassosimone/textwrapper
```

## Development

To run the tests:
```sh
go test -v .
```

To measure test coverage:
```sh
go test -v -cover .
```

## License

```
SPDX-License-Identifier: GPL-3.0-or-later
```

## History

Adapted from [bassosimone/clip](https://github.com/bassosimone/clip/tree/v0.8.0).
