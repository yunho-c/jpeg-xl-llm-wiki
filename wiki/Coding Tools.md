# Coding Tools

JPEG XL combines multiple coding approaches and image-model choices. This page
is the future hub for technical details such as VarDCT, modular coding, color
transforms, progressive decoding, and lossless JPEG recompression.

## Key Points

- Track coding-tool details separately from high-level format claims.
- Do not infer normative behavior from marketing summaries; attach detailed
  claims to libjxl docs, standard text, papers, or implementation code.
- Lossless JPEG recompression deserves special attention because it is a major
  migration feature: existing JPEG images can be represented in JPEG XL and
  restored to equivalent JPEG data.

## Details

Topics to expand as sources are ingested:

- VarDCT mode and photographic image compression.
- Modular mode and lossless or near-lossless coding.
- XYB and perceptual color modeling.
- Entropy coding and transforms.
- Progressive decoding and previews.
- Color management, HDR, and wide-gamut behavior.
- Lossless transcoding from existing JPEG images.

## Sources

- `sources/jpeg-org-jpeg-xl.md`
- `sources/libjxl-format-overview.md`

## Related Pages

- [[Specification]]
- [[libjxl]]
- [[Comparisons]]
- [[Use Cases]]
