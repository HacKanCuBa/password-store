# Emacs password-store

This package provides functions for working with passh ("the standard
Unix password manager").

http://passh.hackan.net

## Setup

The passh application must be installed and set up. See the passh
website for instructions

## Example usage

Interactive:

    M-x password-store-insert
    Password entry: example
    Password: ........
    Confirm password: ........

    M-x password-store-copy
    Password entry: example
    Copied example to the kill ring. Will clear in 45 seconds.
    Password cleared.

Lisp:

    (password-store-insert "example" "password")
    (password-store-get "example") ; Returns "password"
