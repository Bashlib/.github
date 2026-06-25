# Bashlib

A psuedo package management system for the bash scripting language.

## Why bashlib

Are you tired of having duplicate code, crazy source paths, or copying and pasting functions between bash scripts? Well no more! enter bashlib, this tool alows developers to define a `tool.toml` file that bashlib can use to recognize a project as a valid bash package. Projects with a `tool.toml` can be used as dependencies in other bashlib projects and `bashlib-installer` will properly pull the required package and install it locally to your machine on `PATH`. Allowing for easy reuse of bash projects. 

## Bashlib STDLib

These are the packages that are considered part of the bashlib std library. Packages out side of this list should be properly vetted before using in any project. This is a **use at your own risk** system and is best for personal development, any packages not listed in the bashlib std are not guaranteed to be secure or safe. 

### `bashlib-installer`

used to install update and remove bashlib packages. see `bashlib-installer --help`

### `bashlib-create`

used to template bashlib projects and files see `bashlib-create --help`

### `bashlib-style`

used to create a consistent output style for both help menu and different types of debug info see `bashlib-style --help`

### `bashlib-assert`

a testing framework for bash it mostly just simplifies calls to the bash `test` built in.  see `bashlib-assert --help`

### `bashlib-toml`

used to read and write toml in bash. useful when working with the `tool.toml` files or wanting to use TOML as a config file in a project. see `bashlib-toml --help`


## How to use

To create a bashlib project simply use `bashlib-create` this can be used to generate a template project with the required layout and `tool.toml` file. This is the recommended and easiest way to get started.
