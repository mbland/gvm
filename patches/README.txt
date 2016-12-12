Patches for Go builds that apply to all host platforms are stored in each minor
version directory, e.g. go1.4, go1.5, etc.

Patches for platform-specific Go builds are stored in a directory for that
platform, and then by each minor version directory, e.g. alpine/go1.4,
alpine/go1.5, etc.

The patched file paths must all begin with `a/src/` and `b/src/`, as they will
be applied from the `src/` directory of the Go source distribution using `patch
-p2`.
