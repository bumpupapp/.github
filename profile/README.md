# 📦🏷bumpup

**fully automated and extensible software versioning**

[![bumpup](https://img.shields.io/badge/%F0%9F%93%A6-bumpup-informational)](https:/github.com/danielr1996/bumpup)
[![License: ISC](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![deno](https://img.shields.io/badge/deno-v1.26-green.svg?style=round-square&logo=deno)](https:/github.com/danielr1996/bumpup)
[![Build & Release](https://github.com/bumpupapp/bumpup/actions/workflows/build.yaml/badge.svg)](https://github.com/bumpupapp/bumpup/actions/workflows/build.yaml)

[//]: # ([![Maintainability]&#40;https://api.codeclimate.com/v1/badges/fd8a4816eab9e39b70cf/maintainability&#41;]&#40;https://codeclimate.com/github/bumpupapp/bumpup/maintainability&#41;)
[//]: # ([![Test Coverage]&#40;https://api.codeclimate.com/v1/badges/fd8a4816eab9e39b70cf/test_coverage&#41;]&#40;https://codeclimate.com/github/bumpupapp/bumpup/test_coverage&#41;)

> 📦 If you just want to see how to use `bumpup` head straight to
> [@bumpup/cli](https://github.com/bumpupapp/cli)

Like
[standard-version](https://github.com/conventional-changelog/standard-version#readme),
[release-it](https://github.com/release-it/release-it#readme) or
[semantic-release](https://github.com/semantic-release/semantic-release) but
more configurable.

## Highlights

- configurable
- extensible through plugins
- automated
- monorepo compatible

## Key Concepts

`bumpup` focuses on automating the typical steps involved in software
versioning, which for a simple npm project might be:

- reading the current version from `package.json`
- determining the next version according to `semver`
- writing the version to `package.json`
- generating a `CHANGELOG.md`
- push the changes back to the repository
- publish the new package to npm

While these steps work for most projects there are cases where one step differs
slightly from the default. That's were the plugins come into play: Where other
tools promote an _opinionated_ style of how each step should look `bumpup`
allows you to easily swap out plugins or even write your own if your use cases
is not supported.
