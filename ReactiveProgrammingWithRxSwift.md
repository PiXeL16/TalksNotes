# Reactive Programming with RxSwift
[Talk URL](https://realm.io/news/altconf-scott-gardner-reactive-programming-with-rxswift/)

----

* `Sequence` can be subscribe to.
* `DisposeBag` its used to dispose subscription.
* There are wrappers to all the boilerplate code.
* 40% code that you have to write for the same thing.

## What is reactive Programming
* Modeling a sequence.
* Its been around for two decates.

## What is RxSwift
* Implements patterns, types for the reactive parading.
* Everything is a sequence.
* Everything is Async.
* Functional Reactive Programming FTW.

## Common patterns
* Observer
* Iterator

## Lifecycle of an observable sequence
* Represented by a marble diagram.
* Emits a `next`.
* Emits a `error` and terminates a sequence. And it dies.
* Emits a `completed` when it terminates normally.
* `.on` to add to the sequence.
* `.value` enable to set the `onNext`.
* `debug` operator to debug stuff. Nice! 😃.
* `combineLatest` can combine `Subjects`.
* `takewhile` can validate.
* `scan` is like `reduce`.
