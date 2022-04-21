## Differential Testing

Forge can enable differential testing across languages and implementation using the `ffi` [cheatcode](../cheatcodes/ffi.md).

[Differential testing](https://en.wikipedia.org/wiki/Differential_testing) cross references multiple implementations of the same function by comparing each one's outputs. More formally, imagine we have a function specification `f()`, and two implementations of that specification: `f1()` and `f2()`. We expect `EQ(f1(x), f2(x))` for all x that exist in an appropriate input space and some equality function EQ that appropriately assigns equality per the specification. Some real life examples of this include:
* Comparing optimized or upgraded implementations to their predecessors
* Testing code against known reference implementations
* Confirming compatability with third party tools and dependencies.



