# CLI tool to generate simple passwords

Generates a simple password up to 64 characters, using uppercase and lowercase letters, digits and symbols (if enabled).

## Install

`go build -o $GOPATH/passgen`

## Usage

`passgen --help`

`passgen generate --help`

## Examples

Default flags, password length 15 with symbols:

`passgen generate`

Output > `J3x7_FF]E4HYd3.`


Password length 30 without symbols:

`passgen generate -l=30 -s=false`

Output > `4bPkIAjshaoiJqowtY3qQqm5GNe6DD`


## Tests

Run the tests using

`go test ./password`

or

`go test -v ./...`


## Disclaimer

This password generator does **NOT** implement high entropy strategies and should not be used to extreme security requirement applications.
