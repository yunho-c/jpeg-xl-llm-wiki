# Specification

JPEG XL is standardized as ISO/IEC 18181. For wiki maintenance, separate the
normative specification from explanatory materials, reference implementation
behavior, and ecosystem support claims.

## Key Points

- The official JPEG overview identifies JPEG XL as ISO/IEC 18181.
- The specification family includes separate parts for the core coding system,
  file format, conformance testing, and reference software.
- Source cards should distinguish ISO/JPEG committee material from libjxl
  documentation, because implementation behavior can be more concrete than the
  high-level standard overview but is not always a substitute for normative
  language.

## Details

Important specification topics for future ingestion:

- Codestream structure and file/container structure.
- Image metadata, color management, and orientation.
- Lossy and lossless coding modes.
- Progressive decoding and responsive delivery.
- Animation, alpha, layers, previews, and thumbnails.
- Conformance requirements and reference software.

Avoid claiming exact bitstream constraints or syntax rules until a source card
points to the relevant normative or reference documentation.

## Sources

- `sources/jpeg-org-jpeg-xl.md`

## Related Pages

- [[JPEG XL Overview]]
- [[Coding Tools]]
- [[libjxl]]
- [[Open Questions]]
