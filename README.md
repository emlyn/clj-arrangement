Arrangement
===========

[![Circle CI](https://img.shields.io/circleci/project/github/greglook/clj-arrangement.svg?style=flat-square)](https://circleci.com/gh/greglook/clj-arrangement)
[![codecov.io](https://img.shields.io/codecov/c/github/greglook/clj-arrangement.svg?style=flat-square&branch=master)](https://codecov.io/github/greglook/clj-arrangement)
[![API codox](https://img.shields.io/badge/doc-API-blue.svg)](https://greglook.github.io/clj-arrangement/api/)

A micro-library which provides a total-ordering comparator for Clojure values.

## Usage

Library releases are published on Clojars. To use the latest version with
Leiningen, add the following dependency to your project definition:

[![Clojars Project](http://clojars.org/mvxcvi/arrangement/latest-version.svg)](http://clojars.org/mvxcvi/arrangement)

In your code:

```clojure
=> (require '[arrangement.core :as order])

=> (sort order/rank
         ['a false 2 :b nil 3.14159 "c" true \d [3 2] #{:one :two} [3 1 2] #{:three}])
[nil false true 2 3.14159 \d "c" :b a [3 1 2] [3 2] #{:three} #{:one :two}]
```

## License

This is free and unencumbered software released into the public domain.
See the UNLICENSE file for more information.
