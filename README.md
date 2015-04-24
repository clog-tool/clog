clog
====

[![Join the chat at https://gitter.im/thoughtram/clog](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/thoughtram/clog?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Build Status](https://travis-ci.org/thoughtram/clog.png?branch=master)](https://travis-ci.org/thoughtram/clog)

A [conventional](https://github.com/ajoslin/conventional-changelog/blob/master/CONVENTIONS.md) changelog for the rest of us

### Usage

```
USAGE:
    clog [FLAGS] [OPTIONS]

FLAGS:
        --from-latest-tag    use latest tag as start (instead of --from)
    -h, --help               Prints help information
        --major              Increment major version by one (Sets minor and patch to 0)
        --minor              Increment minor version by one (Sets patch to 0)
        --patch              Increment patch version by one
    -v, --version            Prints version information

OPTIONS:
        --from=from                 e.g. 12a8546
    -r, --repository=repository     e.g. https://github.com/thoughtram/clog
        --setversion=setversion     e.g. 1.0.1
        --subtitle=subtitle         e.g. crazy-release-title
        --to=to                     e.g. 8057684 (Defaults to HEAD when omitted)

```

Try it!

1. Clone the repo `git clone https://github.com/thoughtram/clog && cd clog`

2. Build clog `cargo build --release`

3. Delete the old changelog file `rm changelog.md`

3. Run clog `./target/release/clog --repository=https://github.com/thoughtram/clog --setversion=0.1.0 --subtitle=crazy-dog`

## LICENSE

clog is licensed under the MIT Open Source license. For more information, see the LICENSE file in this repository.
