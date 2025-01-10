# Course Prospectus

These are the topics we plan to cover, and the time we plan
to spend covering them. This is all very flexible, and will
likely change rapidly.

Times in parens are hours and minutes for the topic. `[day
1]` etc are course days. Links are to associated material.

## Course Days

1. Wednesday 8 January
2. Friday 10 January
3. Monday 13 January
4. Wednesday 15 January
5. Friday 17 January
6. Monday 20 January
7. Wednesday 22 January
8. Friday 24 January

## Schedule (20:55)

* Rust review (10:30)
  * Basic Datatypes [day 1] (2:50)
    * Numbers [[numbers]] (:15)
    * Arrays and slices [[arrays and slices]] (:40)
    * Strings and chars [[strings]] (:30)
      * Unicode, UTF-8, UTF-16 (:15)
      * slices (:15)
    * Structs and enums [structs and enums] (:55)
      * Structs (:15)
      * Enums (:20)
      * Method syntax and semantics (:20)
    * Exercise: [Rule 110] (:30)
  * Ownership, lifetimes and borrowing [day 2] (2:25)
    * Rust memory model [[memory and moves]] (:15)
    * Move semantics [[memory and moves]] (:15)
    * Memory management (:55)
      * `Box`, mutability [[smart pointers]] (:10)
      * `RefCell` and `Mutex` [[interior mutability]] (:30)
      * `Rc` and `Arc` [[smart pointers]] (:15)
    * Globals, `'static`, leaking (:30)
    * Live Coding: Histograms (:30)
  * Rust types and generics [day 3] (2:35)
    * Generics (1:00)
      * Basic generics [[generics]] (:20)
      * Type aliases [[typedef]] (:10)
      * Const generics (:10)
      * Generic lifetimes (:20)
    * Pattern Matching [[patterns]] (:20)
    * Traits [[traits]] (:45)
      * Trait basics (:20)
      * Associated types (:15)
      * Trait inheritance (:10)
    * Exercise (:30)
  * Generic object programming [day 4] (2:40)
    * Fancy traits (1:10)
      * Trait objects [[trait objects]] (:30)
      * Operator traits [[operators]] (:20)
      * Deref and related traits [[deref]] (:20)
    * Closures and iterators (1:00)
      * Closures [[closures]] (:30)
      * Iterators [[iterators]] (:30)
    * Exercise (:30)

* Software development [day 5] (2:45)
  * Error Handling [[errors]] (:30)
  * Code Checking and Testing [[testing]] (:15)
  * Crates and modules (:30)
    * Module structuring [[modules]] (:15)
    * "Special" crate types (:15)
  * Libraries (:40)
    * Cargo and `crates.io` (:25)
    * `std` and `core` (:15)
  * Stability (:35)
    * Semantic versioning [[semver]] (:10)
    * API stability [[stable]] (:15)
    * Editions [[editions]] (:10)
  * Exercise (:15)

* Unsafe and Embedded [day 6] (2:30)
  * Unsafe fundamentals [[unsafe]] (:30)
    * Basics, safety docs (:15)
    * Nightly (:5)
    * Miri (:10)
  * Embedded programming [[embedded]] (:50)
    * `nostd` (:15)
    * PAC (:15)
    * HAL (:20)
  * Peripheral sharing (:20)
    * `Arc, Mutex` (:10)
    * `PeripheralRef` [[peripheral_ref]] (:10)
  * FFI [[ffi]] (:20)
  * Exercise (:30)

* Async/await [[async-await]] [day 7] (2:45)
  * Top-half: user view (:45)
  * Bottom-half: implementor view (:30)
  * Embassy [[embassy]] (1:00)
    * Embassy basics (:30)
    * Embassy async/await (:30)
  * Exercise (:30)

* Rust Design Patterns [day 8] (2:25)
  * Trait Sealing [[trait sealing]] (:15)
  * Marker Traits (1:10)
    * `Copy` (:20)
    * `Sized` (:10)
    * `Send` and `Sync` (:20)
    * `PhantomData` (:20)
  * Typestate Driven Programming [[typestate]] (:30)
  * Exercise (:30)

---

[numbers]: https://github.com/trifectatechfoundation/teach-rs/blob/main/content/mods/A-foundations/topics/basic-syntax/slides.md
[strings]: https://github.com/pdx-cs-rust/rust-course-notes/blob/main/02-basics/02-4-strings.md
[arrays and slices]: https://github.com/pdx-cs-rust/rust-course-notes/blob/main/02-basics/02-3-aggtypes.md
[structs and enums]: https://github.com/trifectatechfoundation/teach-rs/blob/main/content/mods/A-foundations/topics/composite-types/slides.md
[memory and moves]: https://github.com/trifectatechfoundation/teach-rs/blob/main/content/mods/A-foundations/topics/move-semantics/slides.md
[interior mutability]: https://google.github.io/comprehensive-rust/borrowing/interior-mutability.html
[smart pointers]: https://google.github.io/comprehensive-rust/smart-pointers.html
[generics]: https://github.com/pdx-cs-rust/rust-course-notes/blob/main/old/04-4-generics.md
[typedef]: https://google.github.io/comprehensive-rust/user-defined-types/aliases.html
[patterns]: https://google.github.io/comprehensive-rust/pattern-matching.html
[traits]: https://google.github.io/comprehensive-rust/methods-and-traits/traits.html
[trait objects]: https://github.com/trifectatechfoundation/teach-rs/blob/main/content/mods/A-foundations/topics/trait-objects/slides.md
[operators]: https://github.com/pdx-cs-rust/rust-course-notes/blob/main/old/05-2-op-traits.md
[deref]: https://github.com/pdx-cs-rust/rust-course-notes/blob/main/old/05-4-share-traits.md
[closures]: https://github.com/pdx-cs-rust/rust-course-notes/blob/main/old/06-1-closures.md
[iterators]: https://google.github.io/comprehensive-rust/iterators
[errors]: https://google.github.io/comprehensive-rust/error-handling
[testing]: https://github.com/trifectatechfoundation/teach-rs/blob/main/content/mods/B-crate-engineering/topics/testing/slides.md
[modules]: https://google.github.io/comprehensive-rust/modules
[semver]: https://doc.rust-lang.org/cargo/reference/semver.html
[stable]: https://rust-lang.github.io/api-guidelines/necessities.html#c-stable
[editions]: https://doc.rust-lang.org/edition-guide/
[unsafe]: https://google.github.io/comprehensive-rust/unsafe-rust
[embedded]: https://rust-embedded.github.io/discovery-mb2
[peripheral_ref]: https://docs.embassy.dev/embassy-stm32/git/stm32f102rb/struct.PeripheralRef.html
[ffi]: https://github.com/trifectatechfoundation/teach-rs/blob/main/content/mods/E-rust-for-systems/topics/ffi/slides.md
[async-await]: https://github.com/trifectatechfoundation/teach-rs/tree/main/content/mods/C-multitasking
[embassy]: https://embassy.dev/book/
[trait sealing]: https://predr.ag/blog/definitive-guide-to-sealed-traits-in-rust/
[typestate]: https://cliffle.com/blog/rust-typestate/
[Rule 110]: https://github.com/MasseyRustTraining/rule-110
