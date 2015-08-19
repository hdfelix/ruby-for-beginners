# Numbers

Numbers are simply numbers. You create one by writing it: `12.34` is Ruby code
and it represents the number twelve-point-three-four.

You can also use a comma to separate thousands places: E.g. `1,234.56` is the
number one-thousand-two-hundred-thirty-four-point-five-six.  However, this is
optional. This is the exact same number in Ruby: `1234.56`.

<p class="hint">
A number is defined by a series of digits, using a dot as a decimal mark, and
optinally a comma as a thousands separator.
<p>

Note that different countries use different punctuation for decimal and
thousands separators. Ruby is using the same notation used in the USA, which
happens to be the exact opposite of what's used in Germany.

## Kinds of numbers

Under the hood, for reasons that are mostly technical, there are actually
different kinds of numbers:

For example there are integer numbers (those without a fraction, i.e. a dot and
decimal places), and depending on their size there are two kinds of them. For
floating point numbers there are even more. Unless you are super curious, you
can perfectly ignore all of that for now, and just think of numbers as numbers.

However, when you do calculations with numbers, keep in mind that integer
numbers ("integers") and decimal point numbers (floating point numbers, aka
"floats") are different.

If you do a calculation that starts with an integer you'll eventually always
get an integer back:

```ruby
$ irb
> 1 + 2.0
=> 3
```

And if you start the expression with a float then you'll get a float back:

```ruby
$ irb
> 1.0 + 2
=> 3.0
```

This is, for example, important when you do a division (`/` means "divide by"):

```ruby
$ irb
> 3 / 2
=> 1
```

As you can see any decimal places will be just cut off, since the result needs
to be an integer number.

However, if you start with a float:

```ruby
$ irb
> 3.0 / 2
=> 1.5
```

Exercises: How about doing some of the [exercises on numbers](/exercises/numbers.html)
next?