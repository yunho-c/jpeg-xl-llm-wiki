# JPEG XL Overview

JPEG XL is a still-image coding system standardized as ISO/IEC 18181 and aimed
at both web delivery and high-fidelity imaging workflows. The format combines
lossy and lossless compression, support for modern image features, and a
migration path for existing JPEG images through lossless JPEG recompression.

## Key Points

- JPEG XL should be tracked as three things at once: a specification family, a
  practical file format, and an ecosystem of implementations and platform
  support.
- Official JPEG material positions JPEG XL for web distribution, professional
  photography, wide color gamut, high dynamic range, animation, alpha, layers,
  thumbnails, and efficient decoding.
- The reference implementation is [[libjxl]], which provides libraries,
  command-line tools, documentation, benchmark tooling, and conformance-related
  code.
- Adoption and support are volatile and must be dated. See
  [[Adoption and Support]] before making platform claims.

## Details

The official JPEG overview describes JPEG XL as a royalty-free raster graphics
format with both lossy and lossless modes, designed to supersede legacy JPEG in
many contexts while preserving an efficient path for existing JPEG content. The
specification is split into parts covering the core coding system, file format,
conformance testing, and reference software.

The wiki should not treat JPEG XL only as a browser image format. The same
technical features matter differently across web performance, image archival,
photography, image editing, HDR delivery, and cloud storage.

## Sources

- `sources/jpeg-org-jpeg-xl.md`
- `sources/libjxl-github.md`

## Related Pages

- [[Specification]]
- [[Coding Tools]]
- [[libjxl]]
- [[Adoption and Support]]
- [[Use Cases]]
