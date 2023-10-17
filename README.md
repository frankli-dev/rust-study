# rust-study

### 1. What is the name of the command-line tool for managing the version of Rust on your machine?
rustup

### 2. Every executable Rust program must contain a function with the name:
main

### 3. Let's say you have the following program in a file hello.rs:
```
fn main() {
  println!("Hello world!");
}
```
Say you then run the command rustc hello.rs from the command-line. Which statement best describes what happens next?

Response
- [x] rustc generates a binary executable named hello
- [ ] rustc reformats hello.rs according to the Rust style guide
- [ ] rustc will print an error because this is an invalid program
- [ ] rustc executes the program and prints out Hello world!

### 4. Say you just downloaded a Cargo project, and then you run cargo run at the command-line. Which statement is NOT true about what happens next?

Response
- [x] Cargo watches for file changes and re-executes the binary on a change
- [ ] Cargo downloads and builds any dependencies of the project
- [ ] Cargo executes the project's binary
- [ ] Cargo builds the project into a binary in the target/debug directory
