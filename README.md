# Shell Script Memory Management Bug

This repository demonstrates a common bug in shell scripting: inefficient memory management when handling large files. The `bug.sh` script attempts to read an entire file into memory at once, which can lead to out-of-memory errors for large files.  The `bugSolution.sh` script provides a more efficient solution using a line-by-line processing approach.

**Bug:**
The original script reads the entire file into an array, consuming significant memory.  This approach is unsuitable for files exceeding available RAM.

**Solution:**
The solution script iterates through the file line by line using a `while` loop and `read`, avoiding excessive memory consumption.