# FreeType for Zig

FreeType 2.14.3 with Zig wrappers for libraries, faces, glyphs, and font tables.
Requires Zig 0.17.0.

```sh
zig build
zig build test
zig build test -Denable-libpng=true
zig build test -Denable-libpng=true -Doptimize=safe
```

The package exports the `freetype` module and static `freetype` artifact.
`enable-libpng` enables PNG glyph support (default false).
The build supplies zlib and optional libpng. C declarations use `translate-c`.

The existing memory-font tests use the pinned JetBrains Mono v2.304 font source,
which retains its own OFL license.

Upstream packaging: <https://github.com/allyourcodebase/freetype>.
FreeType: <https://freetype.org/>.
