# Rust-projects
This is where I will be updating my rust projects. This will most likely be embedded systems related.

In the No-std file we are disabling the std since the driver code cannot not depend on it as the std depends on the Os. Guess what the Os depends on .....The driver
Disabling the Std leads to 3 errors;
1. Cannot find println macro
2. #[panic_handler] is required but it is not found.
3. Unwinding panics are not supported without std.

Handling the first error:
<h1 style : "color = green">First Error</h1>
Easy peasy lemon squeezy - comment out the println!("Hello world")
