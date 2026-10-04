# C Data Structures

A study collection of sequential lists, linked support structures, heaps, binary trees, and sorting implementations in C.

```text
include/   Original headers (including the historical spelling Hearp.h)
src/       Implementations
examples/  Original demonstration entry points with descriptive filenames
docs/      File mapping and validation record
```

## Verified example

Build only the sequence-list example from the repository root:

```sh
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug
cmake --build build
./build/sequence_list_demo
```

The existing example inserts `1` and `2`, then prints them. This demonstrates the build path; it is not a comprehensive correctness or memory-management test.

## Historical modules

The binary-tree example requires console input. The heap top-k example expects a local `data.txt`; its data-generation function can create a large file. Neither is run by the cleanup.

`src/Sort.c` and `examples/sorting_demo.c` include `stack2.h`, which was not present in the original repository. These modules are retained for future repair and excluded from the verified CMake target.

Original source bytes and comments are preserved. Some comments use a legacy encoding. See [file mapping](docs/catalog.md) and [validation](docs/validation.md).
