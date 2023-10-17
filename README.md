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

### 5. Which statement best describes what it means if a variable x is immutable?
Response
- [ ] After being defined, x can be changed at most once.
- [ ] x is stored in the immutable region of memory.
- [x] x cannot be changed after being assigned a value.
- [ ] You cannot create a reference to x.

### 6. What is the keyword used after let to indicate that a variable can be mutated?
mut

### 7. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed.
```
fn main() {
  let x = 1;
  println!("{x}");
  x += 1;
  println!("{x}");
}
```

- [ ] This program:  DOES compile
- [x] This program:  does NOT compile

### 8. Which of the following statements is correct about the difference between using let and const to declare a variable?
Response
- [ ] A const can only be assigned to a literal, not an expression involving computation
- [ ] They are just different syntaxes for declaring variables with the same semantics
- [ ] The compiler will error if a const variable's name is not using UPPER_SNAKE_CASE
- [x] const can be used in the global scope, and let can only be used in a function

### 9. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed.
```
fn main() {
  let mut x: u32 = 1;
  {
    let mut x = x;
    x += 2;
  }
  println!("{x}");
}
```
1
### 10. Determine whether the program will pass the compiler. If it passes, write the expected output of the program if it were executed.
```
fn main() {
  let mut x: u32 = 1;
  x = "Hello world";
  println!("{x}");
}
```
Not compile
