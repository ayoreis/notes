# Programming languages

## Functional

- Haskell
- https://ocaml.org
- Lisp
- C 
- C++
- 

- https://vlang.io
- JavaScript
	- https://coffeescript.org
	- https://hegel.js.org
	- https://typescriptlang.org
		- https://civet.dev
- https://python.org
	- https://www.modular.com/mojo
- https://www.erlang.org
- https://elixir-lang.org
- https://www.ruby-lang.org
- [PureScript](https://www.purescript.org)

## Object oriented

## Ideas

- Zero cost abstractions

https://youtu.be/v6RxJsk8otY

```rust
enum Option<T> {
	None,
	Some(T),
}

enum Result<T, E> {
	Ok(T),
	Error(E),
}
```

```typescript
if (condition1) {
	// do 1
} else if (condition2) {
	// do 2
} else if (condition3) {
	// do 3
} else {
	// Runs if none matched
} else {
	// Runs if any matched/else did not
}
```