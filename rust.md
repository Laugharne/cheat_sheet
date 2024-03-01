[Rust Ultimate: The Only Cheatsheet You Will Ever Need for Rust | by Atharva Pandey | Feb, 2024 | Medium](https://medium.com/@gopherine/rust-ultimate-the-only-cheatsheet-you-will-ever-need-for-rust-3cc4798f4109)

# Rust Ultimate: The Only Cheatsheet You Will Ever Need for Rust


## Vector & Linked List Operations

| Data Structure | Method        | Time Complexity | Space Complexity | Description                                                |
| -------------- | ------------- | --------------- | ---------------- | ---------------------------------------------------------- |
| `Vec<T>`       | `new()`       | O(1)            | O(1)             | Creates a new empty vector.                                |
|                | `push(value)` | Amortized O(1)  | O(1)             | Adds an element to the end of the vector.                  |
|                | `pop()`       | O(1)            | O(1)             | Removes the last element from the vector and returns it.   |
|                | `get(index)`  | O(1)            | O(1)             | Returns a reference to the element at the specified index. |


| Data Structure | Method              | Time Complexity | Space Complexity | Description                                         |
| -------------- | ------------------- | --------------- | ---------------- | --------------------------------------------------- |
| `VecDeque`     | `new()`             | O(1)            | O(1)             | Creates a new empty double-ended queue.             |
|                | `push_front(value)` | Amortized O(1)  | O(1)             | Inserts an element at the front of the deque.       |
|                | `push_back(value)`  | Amortized O(1)  | O(1)             | Inserts an element at the back of the deque.        |
|                | `pop_front()`       | O(1)            | O(1)             | Removes and returns the first element of the deque. |
|                | `pop_back()`        | O(1)            | O(1)             | Removes and returns the last element of the deque.  |
| `LinkedList`   | `new()`             | O(1)            | O(1)             | Creates a new empty linked list.                    |
|                | `push_front(value)` | O(1)            | O(1)             | Inserts an element at the beginning of the list.    |
|                | `push_back(value)`  | O(1)            | O(1)             | Inserts an element at the end of the list.          |
|                | `pop_front()`       | O(1)            | O(1)             | Removes and returns the first element of the list.  |
|                | `pop_back()`        | O(1)            | O(1)             | Removes and returns the last element of the list.   |


## HashMap Operations

| Data Structure | Method        | Time Complexity | Space Complexity | Description                                                |
| -------------- | ------------- | --------------- | ---------------- | ---------------------------------------------------------- |
| `HashMap`      | `new()`       | O(1)            | O(1)             | Creates a new empty hash map.                              |
|                | `insert(k,v)` | Average O(1)    | O(1)             | Inserts a key-value pair into the map.                     |
|                | `get(&k)`     | Average O(1)    | O(1)             | Returns a reference to the value corresponding to the key. |
|                | `remove(&k)`  | Average O(1)    | O(1)             | Removes a key from the map and returns its value.          |


## HashSet Operations

| Data Structure | Method             | Time Complexity | Space Complexity | Description                         |
| -------------- | ------------------ | --------------- | ---------------- | ----------------------------------- |
| `HashSet`      | `new()`            | O(1)            | O(1)             | Creates a new empty hash set.       |
|                | `insert(value)`    | Average O(1)    | O(1)             | Adds a value to the set.            |
|                | `contains(&value)` | Average O(1)    | O(1)             | Checks if the set contains a value. |
|                | `remove(&value)`   | Average O(1)    | O(1)             | Removes a value from the set.       |


## String Operations

| Data Structure | Method             | Time Complexity | Space Complexity | Description                                                                      |
| -------------- | ------------------ | --------------- | ---------------- | -------------------------------------------------------------------------------- |
| `String`       | `new()`            | O(1)            | O(1)             | Creates a new empty string.                                                      |
|                | `push_str(s)`      | Amortized O(1)  | O(1)             | Appends a string slice to the end of the string.                                 |
|                | `pop()`            | O(1)            | O(1)             | Removes the last character from the string and returns it.                       |
|                | `trim()`           | O(n)            | O(1)             | Returns a string slice with leading and trailing whitespace removed.             |
|                | `split(delimiter)` | O(n)            | O(1)             | Returns an iterator over substrings of the string, split by the given delimiter. |


## Iterator Operations

| Data Structure | Method          | Time Complexity | Space Complexity | Description                                                                      |
| -------------- | --------------- | --------------- | ---------------- | -------------------------------------------------------------------------------- |
| Iterators      | `map(f)`        | Lazy            | O(1)             | Applies function `f` to each element of the iterator.                            |
|                | `filter(p)`     | Lazy            | O(1)             | Filters elements of the iterator based on predicate `p`.                         |
|                | `fold(init, f)` | O(n)            | O(1)             | Reduces the iterator to a single value using the initial value and function `f`. |
|                | `collect()`     | O(n)            | O(n)             | Transforms the iterator into a collection.                                       |
|                | `zip(it)`       | Lazy            | O(1)             | Zips two iterators into a single iterator of pairs.                              |
|                | `chain(it)`     | Lazy            | O(1)             | Chains two iterators together into a single iterator.                            |


## Advanced Iterator Methods

| Data Structure / Trait | Method          | Time Complexity | Space Complexity | Description                                             |
| ---------------------- | --------------- | --------------- | ---------------- | ------------------------------------------------------- |
| Iterators              | `take(n)`       | O(1)            | O(1)             | Creates an iterator that yields its first `n` elements. |
|                        | `skip(n)`       | O(1)            | O(1)             | Creates an iterator that skips the first `n` elements.  |
|                        | `enumerate()`   | O(1)            | O(1)             | Adds a counter to each item of the iterator.            |
|                        | `peekable()`    | O(1)            | O(1)             | Converts the iterator into a peekable iterator.         |
|                        | `filter_map(f)` | O(n)            | O(1)             | Filters and maps the iterator by a function `f`.        |


## Binary Heap Operations

| Data Structure | Method        | Time Complexity | Space Complexity | Description                                             |
| -------------- | ------------- | --------------- | ---------------- | ------------------------------------------------------- |
| `BinaryHeap`   | `new()`       | O(1)            | O(1)             | Creates a new empty binary heap.                        |
|                | `push(value)` | O(log n)        | O(1)             | Adds an element to the binary heap.                     |
|                | `pop()`       | O(log n)        | O(1)             | Removes and returns the maximum element of the heap.    |
|                | `peek()`      | O(1)            | O(1)             | Returns a reference to the maximum element of the heap. |


## B-Tree Map Operations

| Data Structure | Method               | Time Complexity | Space Complexity | Description                                                |
| -------------- | -------------------- | --------------- | ---------------- | ---------------------------------------------------------- |
| `BTreeMap`     | `new()`              | O(1)            | O(1)             | Creates a new empty B-tree map.                            |
|                | `insert(key, value)` | O(log n)        | O(1)             | Inserts a key-value pair into the map, maintaining order.  |
|                | `get(&key)`          | O(log n)        | O(1)             | Returns a reference to the value corresponding to the key. |
|                | `remove(&key)`       | O(log n)        | O(1)             | Removes a key from the map, maintaining order.             |


## B-Tree Map Operations

| Data Structure | Method             | Time Complexity | Space Complexity | Description                                      |
| -------------- | ------------------ | --------------- | ---------------- | ------------------------------------------------ |
| `BTreeSet`     | `new()`            | O(1)            | O(1)             | Creates a new empty B-tree set.                  |
|                | `insert(value)`    | O(log n)        | O(1)             | Adds a value to the set, maintaining order.      |
|                | `contains(&value)` | O(log n)        | O(1)             | Checks if the set contains a value.              |
|                | `remove(&value)`   | O(log n)        | O(1)             | Removes a value from the set, maintaining order. |


## Option and Result Types

| Data Structure | Method           | Time Complexity | Space Complexity | Description                                          |
| -------------- | ---------------- | --------------- | ---------------- | ---------------------------------------------------- |
| `Option`       | `is_some()`      | O(1)            | O(1)             | Returns `true` if the option is a `Some` value.      |
|                | `is_none()`      | O(1)            | O(1)             | Returns `true` if the option is a `None` value.      |
|                | `unwrap()`       | O(1)            | O(1)             | Unwraps an option, yielding the content of a `Some`. |
|                | `unwrap_or(def)` | O(1)            | O(1)             | Returns the contained value or a default.            |
| `Result`       | `is_ok()`        | O(1)            | O(1)             | Returns `true` if the result is an `Ok` value.       |
|                | `is_err()`       | O(1)            | O(1)             | Returns `true` if the result is an `Err` value.      |
|                | `unwrap()`       | O(1)            | O(1)             | Unwraps a result, yielding the content of an `Ok`.   |
|                | `unwrap_or(def)` | O(1)            | O(1)             | Returns the contained `Ok` value or a default.       |


## File and I/O Operations

| Data Structure | Method           | Time Complexity | Space Complexity | Description                                             |
| -------------- | ---------------- | --------------- | ---------------- | ------------------------------------------------------- |
| `File`         | `open(path)`     | O(1)*           | O(1)             | Opens a file in read-only mode.                         |
|                | `create(path)`   | O(1)*           | O(1)             | Creates a new file, truncating it if it already exists. |
|                | `read(&mut buf)` | O(n)*           | O(1)             | Reads bytes from the file into the buffer.              |
|                | `write(&buf)`    | O(n)*           | O(1)             | Writes the buffer's bytes to the file.                  |
| `BufReader`    | `new(reader)`    | O(1)            | O(1)             | Wraps a reader and provides buffering for it.           |
| `BufWriter`    | `new(writer)`    | O(1)            | O(1)             | Wraps a writer and provides buffering for it.           |


## File System Operations

| Data Structure / Trait | Method                      | Time Complexity | Space Complexity | Description                                       |
| ---------------------- | --------------------------- | --------------- | ---------------- | ------------------------------------------------- |
| `std::fs::File`        | `create(path)`              | O(1)*           | O(1)             | Creates a new file or truncates an existing file. |
| `std::fs::DirBuilder`  | `new()`                     | O(1)            | O(1)             | Creates a new `DirBuilder`.                       |
|                        | `create(path)`              | O(1)*           | O(1)             | Creates a directory at the specified path.        |
| `std::fs`              | `read_dir(path)`            | O(1)*           | O(1)             | Reads the contents of a directory.                |
|                        | `remove_file(path)`         | O(1)*           | O(1)             | Removes a file at the specified path.             |
|                        | `copy(source, destination)` | O(n)*           | O(1)             | Copies a file from source to destination.         |


## Concurrency Primitives

| Data Structure       | Method            | Time Complexity | Space Complexity | Description                                                                |
| -------------------- | ----------------- | --------------- | ---------------- | -------------------------------------------------------------------------- |
| `Thread`             | `spawn(f)`        | O(1)            | O(1)             | Creates a new thread of execution.                                         |
| `Mutex`              | `lock()`          | O(1)            | O(1)             | Locks the mutex, blocking the current thread until it is available.        |
| `Arc`                | `new(data)`       | O(1)            | O(1)             | Creates a new atomic reference-counted pointer.                            |
| `mpsc::Sender`       | `send(value)`     | O(1)            | O(1)             | Sends a value to the corresponding receiver.                               |
| `mpsc::Receiver`     | `recv()`          | O(1)            | O(1)             | Blocks the current thread until a value is received.                       |
| `std::sync::atomic`  | Atomic operations | O(1)            | O(1)             | Provides primitive shared-memory communication between threads.            |
| `std::sync::Barrier` | `Barrier::new(n)` | O(1)            | O(1)             | Enables multiple threads to synchronize the beginning of some computation. |


## Asynchronous Programming

| Data Structure / Trait | Method                 | Time Complexity | Space Complexity | Description                                                |
| ---------------------- | ---------------------- | --------------- | ---------------- | ---------------------------------------------------------- |
| `std::future::Future`  | `await`                | O(1)            | O(1)             | Awaits the completion of an asynchronous operation.        |
| `std::task::Poll`      | Used in `Future::poll` | O(1)            | O(1)             | Enum used to represent the return value of `Future::poll`. |


[Google Cache - Rust Ultimate: The Only Cheatsheet You Will Ever Need for Rust | by Atharva Pandey | Feb, 2024 | Medium](http://webcache.googleusercontent.com/search?q=cache:https://medium.com/@gopherine/rust-ultimate-the-only-cheatsheet-you-will-ever-need-for-rust-3cc4798f4109&vwsrc=1)

## Advanced Numerics and Math Operations

| Data Structure / Trait | Method                | Time Complexity | Space Complexity | Description                                  |
| ---------------------- | --------------------- | --------------- | ---------------- | -------------------------------------------- |
| \`std::cmp::Ord\`      | \`cmp(&self, other)\` | O(1)            | O(1)             | Compares two values and returns an ordering. |
| \`std::iter::Sum\`     | \`sum\`               | O(n)            | O(1)             | Sums up all items in the iterator.           |
| \`std::iter::Product\` | \`product\`           | O(n)            | O(1)             | Multiplies all items in the iterator.        |

## Traits and Pattern Matching

| Trait / Feature       | Method / Use Case     | Time Complexity | Space Complexity | Description                                                       |
| --------------------- | --------------------- | --------------- | ---------------- | ----------------------------------------------------------------- |
| \`std::fmt::Debug\`   | \`{:?}\` (formatting) | O(n)            | O(1)             | Formats a value using its debug representation.                   |
| \`std::fmt::Display\` | \`{}\` (formatting)   | O(n)            | O(1)             | Formats a value using its display representation.                 |
| Pattern Matching      | \`match val {}\`      | O(1) - O(n)     | O(1)             | Matches values against patterns and deconstructs them.            |
| Enums and Matching    | \`enum {Variants}\`   | O(1)            | O(1)             | Defines an enumeration and matches its variants in control flows. |

## Traits for Generic Programming

| Trait                     | Method / Associated Function | Time Complexity | Space Complexity | Description                                                 |
| ------------------------- | ---------------------------- | --------------- | ---------------- | ----------------------------------------------------------- |
| \`std::iter::Iterator\`   | \`next()\`                   | O(1)            | O(1)             | Advances the iterator and returns the next value.           |
| \`std::convert::From\`    | \`from()\`                   | O(1)            | O(1)             | Converts a value from one type to another.                  |
| \`std::convert::Into\`    | \`into()\`                   | O(1)            | O(1)             | Consumes the original value, returning the converted value. |
| \`std::default::Default\` | \`default()\`                | O(1)            | O(1)             | Provides a default value for a type.                        |
| \`std::clone::Clone\`     | \`clone()\`                  | O(n)            | O(n)             | Creates a new instance of a type by cloning its content.    |
| \`std::cmp::PartialEq\`   | \`eq(&self, other)\`         | O(1)-O(n)       | O(1)             | Provides functionality for partial equality comparisons.    |

## Advanced Pattern Matching and Enums

| Feature              | Use Case                           | Time Complexity | Space Complexity | Description                                                  |
| -------------------- | ---------------------------------- | --------------- | ---------------- | ------------------------------------------------------------ |
| Enums with \`match\` | \`match enum\_var { ... }\`        | O(1)            | O(1)             | Deconstructs enums in a type-safe way with pattern matching. |
| Pattern Guards       | \`if let Some(x) = expr { ... }\`  | O(1)            | O(1)             | Combines pattern matching with conditional guards.           |
| \`@\` Bindings       | \`match val { pat @ subpat =...}\` | O(1)            | O(1)             | Allows binding a name to a value tested by a deeper pattern. |

## Collections and Their Advanced Uses

| Data Structure / Trait      | Method                    | Time Complexity | Space Complexity | Description                                                              |
| --------------------------- | ------------------------- | --------------- | ---------------- | ------------------------------------------------------------------------ |
| \`std::collections::Range\` | \`start..end\`            | O(1)            | O(1)             | Represents an iterator over a range of values.                           |
| \`std::slice::Slice\`       | \`binary\_search(&self)\` | O(log n)        | O(1)             | Searches for an element in a sorted slice using binary search.           |
| \`std::vec::Vec\`           | \`resize\_with(len, f)\`  | O(n)            | O(n)             | Resizes the vector to the new length with a function to create elements. |

## Error Handling and Debugging

| Feature / Trait                  | Method / Use Case                | Time Complexity | Space Complexity | Description                                                                          |
| -------------------------------- | -------------------------------- | --------------- | ---------------- | ------------------------------------------------------------------------------------ |
| \`std::result::Result\`          | \`map\_err(f)\`                  | O(1)            | O(1)             | Maps a \`Result\` to \`Result\` by applying a function to a contained \`Err\` value. |
| \`std::option::Option\`          | \`and\_then(f)\`                 | O(1)            | O(1)             | Calls a function on the contained value of an \`Option\` or returns \`None\`.        |
| \`std::panic\`                   | \`panic!("msg")\`                | O(1)            | O(1)             | Triggers a panic with a custom message.                                              |
| \`std::dbg!\`                    | \`dbg!(&val)\`                   | O(n)            | O(1)             | Prints and returns the value of a given expression for quick debugging.              |
| \`std::error::Error\`            | \`description()\`                | O(1)            | O(1)             | Provides a description of the error.                                                 |
| \`std::panic::catch\_unwind(f)\` | Try to catch panics within \`f\` | O(1)            | O(1)             | Allows potentially recovering from panics within a given function.                   |

## Time Operations

| Data Structure / Trait  | Method                     | Time Complexity | Space Complexity | Description                                                         |
| ----------------------- | -------------------------- | --------------- | ---------------- | ------------------------------------------------------------------- |
| \`std::time::Instant\`  | \`now()\`                  | O(1)            | O(1)             | Returns an instance of \`Instant\` representing the current moment. |
|                         | \`duration\_since(other)\` | O(1)            | O(1)             | Calculates the duration since a previous instant.                   |
| \`std::time::Duration\` | \`from\_secs(secs)\`       | O(1)            | O(1)             | Creates a new \`Duration\` from a specified number of seconds.      |
|                         | \`as\_secs()\`             | O(1)            | O(1)             | Returns the total number of seconds contained by this duration.     |

## Networking

| Data Structure / Trait    | Method             | Time Complexity | Space Complexity | Description                                                |
| ------------------------- | ------------------ | --------------- | ---------------- | ---------------------------------------------------------- |
| \`std::net::TcpListener\` | \`bind(addr)\`     | O(1)\*          | O(1)             | Binds to the specified address and returns a TCP listener. |
| \`std::net::TcpStream\`   | \`connect(addr)\`  | O(1)\*          | O(1)             | Connects to a TCP listener at the specified address.       |
|                           | \`read(&mut buf)\` | O(n)\*          | O(1)             | Reads data from the TCP stream into the buffer.            |
|                           | \`write(&buf)\`    | O(n)\*          | O(1)             | Writes data from the buffer to the TCP stream.             |

## Meta-programming and Macros

| Feature / Trait              | Use Case                            | Time Complexity | Space Complexity | Description                                                                                               |
| ---------------------------- | ----------------------------------- | --------------- | ---------------- | --------------------------------------------------------------------------------------------------------- |
| Macros                       | \`macro\_rules! macro\_name {...}\` | Compile-time    | -                | Allows writing code that generates other code (metaprogramming).                                          |
| \`std::marker::PhantomData\` | Used in generic types               | -               | O(1)             | Allows indicating phantom type parameters which affect type variance.                                     |
| Declarative Macros           | \`macro\_rules!\`                   | Compile-time    | -                | Allows writing DRY code with pattern matching on macro arguments.                                         |
| Procedural Macros            | Custom derive, \`#\[proc\_macro\]\` | Compile-time    | -                | More flexible macros that operate on the Rust AST for custom traits or attribute-like macros.             |
| Attribute Macros             | \`#\[attribute\_macro\]\`           | Compile-time    | -                | Macros that are applied to modules, functions, or structs to generate or modify code.                     |
| \`std::macro\`               | \`concat!\`, \`env!\`, \`cfg!\`     | Compile-time    | -                | Built-in macros for concatenating literals, accessing environment variables, and conditional compilation. |

## Unsafe Operations

| Feature           | Use Case                                            | Time Complexity | Space Complexity | Description                                                              |
| ----------------- | --------------------------------------------------- | --------------- | ---------------- | ------------------------------------------------------------------------ |
| \`unsafe\` blocks | \`unsafe { ... }\`                                  | -               | -                | Performs operations that the compiler can't guarantee to be safe.        |
| \`std::ptr\`      | \`null()\`, \`is\_null()\`, \`read()\`, \`write()\` | -               | -                | Provides raw pointer functionality, such as dereferencing or arithmetic. |