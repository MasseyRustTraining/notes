# Getting Started With Rust

It's easy enough to get started with Rust on a variety of
platforms. All are fairly similar.

## Getting Started With Rust On Windows

* If you are using an existing code editor or IDE you are
  fond of, look into how to set it up for Rust.  (I use
  emacs, which works… OK.) There are great Rust tutorials
  online for most of these.
  
  If in doubt, install Visual Studio Code from the Microsoft
  App Store. Then install the official `Rust Analyzer`
  plugin from rust-lang.org. Do not install any other Rust
  plugins at this stage: there's some janky stuff floating
  around.  There's some information on setup at

    * https://code.visualstudio.com/docs/languages/rust
    * https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer

* Now go to https://rustup.rs and download and run
  `rustup.exe`. I know this is a bit scary, but it is all
  well protected by PKI and will do nothing less benign than
  install Rust on your machine via Rustup.

  The installer will open a terminal and run on the command
  line: it is fine to hit return and take the defaults for
  the install. Once the installation completes, close the
  terminal, open a new terminal, and say `rustc --version`.
  If all is well, you should see the version number of the
  latest Rust.

* You can now create new Rust programs and libraries with
  `cargo new`:
  
    * Say `cargo new --bin myprogram` to create a Rust program
      called `myprogram`.
    
    * Say `cargo new --lib myprogram` to create a Rust library
      called `myprogram`.

  You may also be able to create new programs and libraries
  from your IDE.

* In VSCode you can File » Open Folder and then navigate to
  a Rust directory to open it as a Rust project.

## Getting Started With Rust On Linux, WSL, Mac

The instructions here can be very similar to the Windows
instructions. Go to `https://rustup.rs` to install Rust,
install whatever IDE / Editor and support you want, and off
you go.
