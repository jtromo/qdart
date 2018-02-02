# qdart

Quick Dart

## Description
Quick Dart provides short, easy to remember commands to make your life using dart and pub easier.

Dependent on your dart project using: [dart_dev](https://pub.dartlang.org/packages/dart_dev)

## Usage
qdart supports both single letter options that will be executed in sequence as well as traditional long arguments. These can be mixed in any order or even repeated.

```
GNU Usage
    ./qdart [options]

POSIX Usage
    ./qdart -[single letter options]

Options
                --clean, -c Clear out pub dependencies. Performs ```rm -rf .pub .packages pubspec.lock &&
                 find . -name packages | xargs rm -rf```. Attempts to go into folders and
                 clean them in there are any pubspec.yaml files.
                --clean-hard Performs all the actions of --clean in addition to clearing pub
                 cache with ```rm -rf ~/.pub-cache```
                --format, -f ```pub run dart_dev format``` of dart code.
                --get, -g Perform a ```pub get``` for pub dependencies. Will attempt to go
                 into directories to find pubspec.yaml files.
                --help, -h Display this usage text.
                --serve, -s Serve dart code using ```pub run dart_dev serve```. Attempts to go into an
                 app directory and serve from there if available.
                --test, -t Test dart code using ```pub run dart_dev test```.
                --upgrade, -u Perform ```pub upgrade``` in directories with a pubspec.yaml.

Examples
    ./qdart -gft
    ./qdart --clean --get --serve
    ./qdart -cgs
    ./qdart -clean -gs
```

## Installation
Can be installed via brew:
```brew install jtromo/homebrew-ember-spark/qdart```
