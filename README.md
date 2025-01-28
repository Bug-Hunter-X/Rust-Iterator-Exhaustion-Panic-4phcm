# Rust Iterator Exhaustion
This repository demonstrates a common error in Rust: attempting to iterate over an iterator after it's exhausted.  The example uses a `Vec` and its iterator.  After all elements are consumed, further calls to `next()` result in a panic.
The solution shows how to handle this by checking for `None` returned by `next()` before proceeding.