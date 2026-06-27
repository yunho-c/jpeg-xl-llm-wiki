# libjxl

libjxl is the JPEG XL reference implementation. It is the practical entrypoint
for encoding, decoding, testing, benchmarking, API behavior, and many examples
used by downstream projects.

## Key Points

- libjxl provides command-line tools, libraries, documentation, examples,
  benchmark tooling, and test data related to JPEG XL.
- `cjxl` and `djxl` are the main command-line tools to track for common encode
  and decode workflows.
- libjxl documentation and source code are primary evidence for implementation
  behavior, but specification claims should still point back to standard or JPEG
  committee sources when possible.
- Licensing and patent-grant claims should be sourced directly to the libjxl
  repository materials.

## Details

Future pages can split out practical guides for:

- Installing and building libjxl.
- Encoding with `cjxl`.
- Decoding with `djxl`.
- Benchmarking JPEG XL against other formats.
- Using the C/C++ APIs.
- Understanding test images, conformance tools, and fuzzing.

## Sources

- `sources/libjxl-github.md`
- `sources/libjxl-format-overview.md`

## Related Pages

- [[JPEG XL Overview]]
- [[Specification]]
- [[Coding Tools]]
- [[Use Cases]]
