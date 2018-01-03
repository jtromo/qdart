# qdart

Quick Dart

## Description
Quick Dart provides short, easy to remember commands to make your life using dart and pub easier.

Dependent on your dart project using: [dart_dev](https://pub.dartlang.org/packages/dart_dev)

## Usage
qdart supports both single letter options that will be executed in sequence as well as traditional long arguements. These can be mixed in any order or even repeated.

```
GNU Usage
    ./qdart [options]

POSIX Usage
    ./qdart -[single letter options]

Options
                --clean, -c Clear out pub dependencies.
                --format, -f Format dart code.
                --get, -g Get pub dependencies.
                --help, -h Display this usage text.
                --serve, -s Serve pub code.
                --test, -t Test pub code.
                --upgrade, -u Upgrade pub dependencies.

Example
    ./qdart --clean --get --serve
    ./qdart -cgs
    ./qdart -clean -gs
```

## Installation
Can be installed via brew:
```brew install jtromo/homebrew-ember-spark/qdart```
