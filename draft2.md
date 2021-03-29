# Effective code comms

### Keywords to determine patterns used
- generate, new, init, make, create are keywords used for creation patterns
- get, traverse, generate, find, look, delete, edit, update, remove, sync, modify are behavioral patterns
- main, start, execute are usually keywords used for structural patterns

### When reading and describing code
1. Find the main function call
1. Looking at the name, you can deduce which of the patterns the code block it belongs to
1. Look at the return value. Typed languages have the advantage over this because usually the return value is declared
1. Just glance over the main body and quickly see what it does

### Talk about the code using the template below
_This function <u>pattern name</u> the <u>return value</u>. It takes in the <u>args</u> as arguments_ ...
