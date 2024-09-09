## Table of Contents

- [Requirements](#requirements)

- [Run Command](#run-command)

## Requirements

To compile and run this project, you need the following:

- **GCC**: Ensure that you have GCC installed for compiling C files.
- **Make**: Required to run the `make` commands.
- **Standard C Libraries**: The project uses several standard C libraries, including:
  - `stdio.h` for standard input/output functions.
  - `stdlib.h` for memory allocation, process control, conversions, and others.
  - `string.h` for string handling functions.
  - `unistd.h` for accessing the POSIX API.
  - `ctype.h` for character handling functions.
  - `stdint.h` for fixed-width integer types.
  - `time.h` for handling time-related functions.
  - `stddef.h` for defining various useful types and macros.
  - `errno.h` for reporting and retrieving error conditions.

- **Networking Libraries**: The project involves network communication, so the following libraries are necessary:
  - `sys/socket.h` for socket programming.
  - `netinet/in.h` for Internet address family.
  - `arpa/inet.h` for handling Internet operations like converting IP addresses.

- **Custom Libraries**:
  - `microtcp.h`: A custom library located in the `lib` directory
  - `crc32.h`: A utility header for CRC32 checksums, located in the `utils` directory.

## Run Command

To run the test run this command in the first terminal:

```bash
make test;./test -s -m -p 54321 -f save.txt
```

and this command in the second terminal:

```bash
./test -m  -p 54321 -a 192.168.1.5 -f big.txt
```
