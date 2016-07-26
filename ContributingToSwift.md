# Contributing to Swift: From Proposal to Shipped
[Talk URL](https://realm.io/news/slug-russ-bishop-contributing-open-source-swift-proposal/)
-----
# Getting Started

* master required Xcode 8
* add your fork to a deferent repo ( not `origin` or `upstream`)

# Building
* use `/utils/build-script`
* Takes a lot of time.. 33 minutes..

# Directory structure
* `include` `lib` most of the compiler C++ * `stdlib` standard library
* `apinotes` rename types, map selectors, etc
* `docs` not up to date.
* `unittest` not the actual unit test
* `test` actual unit tests
* `validation-test`

# Tests
* Use LLVM lit
* Takes like 13 minutes
* Validation tests 1+ hour

# Toolchains
* All the package of tools that allow you to build
* Xcode presents them in the toolchains menu

# Coordination
* swift-evolution
* swift-dev
* bugs.swift.org

# Read
* `Jordan Rose` So you want to be a compiler wizard
* LLVM tutorial llvm.org/docs/tutorial/
