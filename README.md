# Awesome Rust floats

This is a curated list of Rust floating-point crates and utilities. Mostly a list of crates I find interesting.

## Improved precision

- [Accurate](https://crates.io/crates/accurate), implement exact (no round-off) and compensated (improved precision) sum and dot product algorithms plus accumulators
- [Rug](https://crates.io/crates/rug), arbitrary precision numbers with correct rounding (GMP, MPFR bindings)
- [Ramp](https://crates.io/crates/ramp), high performance arbitrary precision int and rationals (floats are in their TODO)
- [Two-float](https://crates.io/crates/twofloat), double double arithmetic (roughly doubled precision)

## Float comparison

- [Approx](https://crates.io/crates/approx), compare floats with absolute or relative values (designed for test suites)
- [Float-comp](https://crates.io/crates/float-cmp), compare float in absolute value or number or ULP
- [Ordered float](https://crates.io/crates/ordered-float), wrapper for floats that makes them ordered and hashable

## Generic code

- [Num traits](https://crates.io/crates/num-traits), traits to implement numerical code generic over types and new numeric types
- [Numeric literals](https://crates.io/crates/numeric_literals), macro to convert literals into a type

## Correctness

- [Uom](https://crates.io/crates/uom), numbers that encode units of measurement
- [Noisy float](https://crates.io/crates/noisy_float), floats that panic when they become Nan
- [Herbie lint for rust](https://github.com/mcarton/rust-herbie-lint), warning on numericaly unstable mathematical expression (*Not functional anymore*)

## IEEE-754 specific operations

- [IEEE754](https://crates.io/crates/ieee754), low level float operations (such as getting the next representable float)
- [Safe EFT](https://crates.io/crates/safeeft), error free transformations (fucntions that can extract the numerical error produced by an operation)

## Alternative numeric types

- [Num](https://crates.io/crates/num), collection of numeric types (and traits) including rationals and complex numbers
- [SoftPosit](https://crates.io/crates/softposit), posit numbers (alternative to IEEE-754 arithmetic)
- [Half](https://crates.io/crates/half), 16 bit float (storage only, no operator provided)

#### Intervals arithmetic

- [Intervallum](https://crates.io/crates/intervallum), interval operations (does not seem to take round-offs into account)
- [Honest intervals](https://crates.io/crates/honestintervals), interval operations (does take round-offs into account)
- [efloat](https://crates.io/crates/efloat), keep track of an upper ad lower bound on the numbers (meant to be used as a check on precision)

#### fixed point numbers

- [Rust_decimal](https://crates.io/crates/rust_decimal), viable for finance
- [Bigdecimal](https://crates.io/crates/bigdecimal), arbitrary precision
- [Fixed](https://crates.io/crates/fixed), basic formats (no algebraic functions)
