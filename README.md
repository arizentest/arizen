[![Dependency status][david-img]][david-url]
[![License][license-img]][license-url]
[![Build status][travis-img]][travis-url]
[![Code Climate][codeclimate-img]][codeclimate-url]
[![Coverage Status][testcoverage-img]][testcoverage-url]

# Arizen
Arizen is ZenCash wallet.

# Version History
## v1.1.1
- [x] Fixed auto-updater issue

## v1.1.0
- [x] New GUI and improved functionality

## v1.0.1
- [x] added possibility to chose one of your wallet in "Send" "To" section
- [x] Fixed bug with wrong transaction ordering in transaction history section
- [x] Fixed bug with importing wallet on "Create new wallet" forms, for `.uawd` and `.awd` files
- [x] Fixed copy/cut/paste in register form
- [x] Allow special character in username
- [x] Fixed auto-update feature on Windows
- [x] Only `AppImage` format is supported for Linux (only this format can be auto-updated)

## v1.0.0
- [x] You can download Arizen wallet from Release section from Github right now
- [x] You can create multiple separate accounts
- [x] Password protected locally stored accounts
- [x] All data are encrypted (any of other wallets does not have this) and stored only on your HDD
- [x] Detailed info about address and transaction history
- [x] You can import / export wallet to encrypted `.awd` / decrypted `.uawd` Arizen's file
- [x] Desktop notifications when balance has been changed
- [x] Arizen automatically downloads updates instead of you
- [x] Windows + MacOS + Linux installation files

## Wallet
- [x] Needs connection to the insight and API (you can change servers in settings)
- [x] Arizen is API wallet

## Development

### How to create distribution
npm run dist

### Coding rules

#### Mostly everything
- Indent with 4 spaces (JS/CSS/HTML)
- Quote with double quotes (JS/CSS/HTML)
- Do not comment unfinished/not working/old code. Use the Git Luke.

#### JavaScript
- Place opening brace on the same line.
- Write names of variables and functions in _lower camel case_, for example

      const totalZenBalance = totalBalance + getTxBalance(tx);

- Write names of classes in _upper camel case_, for example

      class AddressDialog {
	      /* ... */
	  }

- Write constant names in _constant case_, for example

      const UPDATE_INTERVAL = 60; // seconds

- Prefer cloning HTML `<template>`s to constructing DOM trees manually.

#### HTML
- Do not quote _simple_ HTML attribute values. For example write

      <span id=foo class=bar>

  instead of

      <span id="foo" class="bar">

  unless you have to, for example in

      <span id=foo class="bar baz">

- Write identifiers (values of `id`, `class`, `name`, `data-tr`, etc.) in _lower camel case_, for example

      <span id=totalBalance class=bigLabel>

# Screenshots
![Overview of walet](https://i.imgur.com/rQKZ3FL.png)
![Overview of walet 2](https://i.imgur.com/wm4SXkY.png)
![List of addresses](https://i.imgur.com/zCxibuz.png)
![Transaction detail](https://i.imgur.com/4oFREfR.png)
![Settings](https://i.imgur.com/TFfrQMD.png)
![About](https://i.imgur.com/Vb3ao6m.png)

[david-img]: https://david-dm.org/ZencashOfficial/arizen.svg?style=flat-square
[david-url]: https://david-dm.org/ZencashOfficial/arizen
[license-img]: https://img.shields.io/badge/license-MIT-green.svg?style=flat-square
[license-url]: LICENSE
[travis-img]: https://img.shields.io/travis/ZencashOfficial/arizen.svg?style=flat-square
[travis-url]: https://travis-ci.org/ZencashOfficial/arizen.svg?branch=master
[codeclimate-img]: https://codeclimate.com/github/ZencashOfficial/arizen/badges/gpa.svg?style=flat-square
[codeclimate-url]: https://codeclimate.com/github/ZencashOfficial/arizen
[testcoverage-img]: https://coveralls.io/repos/github/ZencashOfficial/arizen/badge.svg?branch=master
[testcoverage-url]: https://coveralls.io/github/ZencashOfficial/arizen?branch=master

