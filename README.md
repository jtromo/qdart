# qdart

Quick Dart

## Description
Quick Dart provides short, easy to remember commands to make your life using dart and pub easier.

Dependent on your dart project using: [dart_dev](https://pub.dartlang.org/packages/dart_dev).

## Usage
qdart supports both single letter options that will be executed in sequence as well as traditional long arguments. These can be mixed in any order or even repeated.

```
GNU Usage
    ./qdart [options]

POSIX Usage
    ./qdart -[single letter options]

Options
        --analyze, -a : runs the `dartanalyzer` over source code.
        --chromium-checked-mode : launches Chromium in checked mode using `DART_FLAGS=--checked open /usr/local/opt/dart/Chromium.app`.
        --clean, -c : clears out pub dependencies. Performs `rm -rf .pub .packages pubspec.lock && find . -name packages | xargs rm -rf`. Attempts to go into directories with pubspec.yaml files.
        --clean-hard: performs all the actions of `--clean` in addition to clearing pub cache with `rm -rf ~/.pub-cache`.
        --copy-license : copies a LICENSE file to all applicable files.
        --coverage : collects coverage over test suites (unit, integration, and functional) and generates a report. Uses the coverage package.
        --docs, d : runs the tool from the `dartdoc` package to generate docs.
        --examples, e : uses `pub serve` to serve the project examples.
        --format, -f : runs the `dartfmt` tool from the `dart_style` package over source code.
        --gen-test-runner : generates a test runner file that allows for faster test execution.
        --get, -g : runs `pub get` for pub dependencies. Will attempt to go into directories to find pubspec.yaml files.
        --get-package-solver : gets and identifies pub dependency issues. Will attempt to go into directories to find pubspec.yaml files.
        --help, -h : displays this usage text.
        --prune, -p : cleans up local branches after they have been merged using `git fetch --prune origin && git branch --merged master | grep -v "\master" | xargs -n 1 git branch -d`.
        --saucelabs : compiles dart unit tests that can be run in the browser and executes them on various platforms using Sauce Labs.
        --serve, -s : uses `pub serve` to serve the project. Attempts to go into an app directory and serve from there if available.
        --serve-dart2js : serves the project using the `dart2js` compilation option to work on non-Chromium browsers.
        --task-runner : uses `task-runner` to perform tasks found on the `config.taskRunnerConfig`
        --test, -t : runs test suites (unit, integration, and functional) via the `test` package test runner.
        --upgrade, -u : runs `pub upgrade` in directories with a pubspec.yaml.

Example
    ./qdart -gft
    ./qdart --clean --get --serve
    ./qdart -cgs
    ./qdart -clean -gs
```

## Contributions
[Contribution guidelines for this project](.github/CONTRIBUTING.md).

## Installation
Can be installed via brew:
```brew tap jtromo/homebrew-ember-spark```
```brew install jtromo/homebrew-ember-spark/qdart```
