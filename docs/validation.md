# Validation record

Date: 2026-10-04. Cleanup baseline commit: `e4ed62371d73022d5a2f2220f270d19c7953a3c2`.

## Preservation and structure

- 16 retained blobs are unchanged at their current paths.
- 0 generated build/cache/executable entries are omitted from the current tree; the baseline history remains available.
- New documents and required configuration/path adaptations are recorded in the cleanup pull request. No existing source history is rewritten.
- Current filenames have no case-insensitive collisions. Markdown file links and generated-output ignore rules are checked before publication.

## Checks and limits

- Apple Clang 21 / C17: `cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug` and `cmake --build build` passed.
- `./build/sequence_list_demo` exited with code 0 and printed `1` and `2`.
- Other algorithms were not executed. Sorting is blocked by missing `stack2.h`; top-k requires local data. This is a smoke check rather than full algorithm or memory-safety validation.

