# C++ Templates

## Local Variable

Aliases for local variable declaration.

- `var`, `letmut` for `auto <var> = <value>;`
- `val`, `let` for `const auto <var> = <value>;`

## FundamentalTypes

Aliases for fundamental types, including integer types and floating-point types.

It's suggested to use these templates since C++ 11. See:

- [Fundamental types - cppreference.com](https://en.cppreference.com/w/cpp/language/types)
- [Fixed width integer types - cppreference.com](https://en.cppreference.com/w/cpp/types/integer)

### Imports

```c++
#include <cstdint>
```

### Basic

File: `./FundamentalTypes-Basic.xml`

> **Note**
> For most platforms, fixed width integer types are available,
> but if you are targeting an old or embedded system, 
> these types may not available,
> use `FastInt` or `LeastInt` below instead.


Rust-style aliases for C++, including:

- Signed integer types: `i{8,16,32,64}` to `int{8,16,32,64}_t` 
in `cstdint`, `i` stands for `integer`.
- Unsigned integer types: `u{8,16,32,64}` to `uint{8,16,32,64}_t`
in `cstdint`, `u` stands for `unsigned`.
- Floating-point types:
    - `f32` to `float`
    - `f64` to `double`
    - `f80`, `f96`, `f128` to `long double`
    - `f` stands for `float`.

### FastInt

File: `./FundamentalTypes-FastInt.xml`

Fast variation of fixed width integer types:

- `{u,i}{8,16,32,64}f` to `u?int_fast{8,16,32,64}_t`,
`f` stands for `fast`.

### LeastInt

File: `./FundamentalTypes-LeastInt.xml`

Least variation of fixed width integer types:

- `{u,i}{8,16,32,64}m` to `u?int_least{8,16,32,64}_t`,
`m` stands for `minimum`.
