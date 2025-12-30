# Golang Text Wrapper with Indent

[![GoDoc](https://pkg.go.dev/badge/github.com/bassosimone/textwrap)](https://pkg.go.dev/github.com/bassosimone/textwrap) [![Build Status](https://github.com/bassosimone/textwrap/actions/workflows/go.yml/badge.svg)](https://github.com/bassosimone/textwrap/actions) [![codecov](https://codecov.io/gh/bassosimone/textwrap/branch/main/graph/badge.svg)](https://codecov.io/gh/bassosimone/textwrap)

The `textwrap` Go package contains code to wrap and indent text.

For example:

```Go
import "github.com/bassosimone/textwrap"

const (
	indent = "    "
	width = 72
)
output := textwrap.Do(paragraph, width, indent)
```

The above example wraps paragraph with the given four spaces
indent such that lines are `<=` 72 chars.

## Installation

To add this package as a dependency to your module:

```sh
go get github.com/bassosimone/textwrap
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
