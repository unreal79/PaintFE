# Codec Investigation

Production HEIC processing uses codecs installed on the system or provided by the user. The earlier decoder experiment, its metadata dependency, benchmark results, and the separate HEVC helper/build setup have been retired. Historical measurements are still in Git history, but they are not current codec recommendations.

The separate AVIF probe still exists under `tools/codec_probe/`. Current app behavior and limits are documented in [HEIC and AVIF](heif-avif.md) and [export settings](export-settings.md). Codec choice must be checked against decoded pixels, alpha handling, precision, malformed files, and memory limits. File size or a thumbnail alone does not prove equivalent output.
