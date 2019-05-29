# String's Split Method, Word Array Literal, and Array's Join Method

## Learning Goals

- Join elements of an `Array` with `join` to produce a `String`
- Create an `Array` of words with Ruby's `%w[]` literal
- Split a `String` into an `Array` of words

## Introduction

At this point in our journey, we're probably really keen to get some more data
than just plain old numbers. It's a good time to cover to methods that are
inverses of each other:

* `String`'s `split`
* `Array`'s `join`

## Join Elements of an `Array` With `join` to Produce a `String`

Since we're in a module about `Array`s, let's talk about joining an `Array` of
words.

```ruby
["This", "is", "a", "test"].join(' ') #=> "This is a test"
["This", "is", "a", "test"].join('_') #=> "This_is_a_test"
["This", "is", "a", "test"].join('*') #=> "This*is*a*test"
```

For more details, consult the [join][] documentation.

## Create an `Array` of Words with Ruby's %w// Literal

Creating an `Array` of words can be difficult to type with all those `"`
characters rolling about. Ruby invented an operator called the Array of Words
literal.

```ruby
%w[this is also a test] #=> ["this", "is", "also", "a", "test"]
# For method-chaining fun:
%w[this is also a test].join(" ").capitalize #=> "This is also a test"
```

## Split a `String` into an `Array` of words

If `Array's` `join` can turn an `Array` of `Strings` into one `String`, we can
reverse the process with `String`'s `split` method:

```ruby
"When in the course of human events".split(" ") #=> ["When", "in", "the", "course", "of", "human", "events"]
```

Here is a bit of Thomas Jefferson's _Declaration of Independence_.

## Conclusion

These methods and the `Array` word literal are tools to help you accomplish
programming tasks when working with text. There's a lot more to learn, but
these are a good start.

## Resources

* [join][join]
* [Array Literal][al]
* [split][split]

[join]:  https://ruby-doc.org/core-2.6.3/Array.html#method-i-join
[split]: https://ruby-doc.org/core-2.6.3/String.html#method-i-split
[al]: https://docs.ruby-lang.org/en/2.6.0/syntax/literals_rdoc.html#label-Percent+Strings
