# GlowLang Examples

Small, complete programs that show how to build things with
[GlowLang](https://github.com/anshumali19/GlowLang-core). Every example here runs with the
current GlowLang release built from GlowLang-core.

| Example | What it shows | Needs |
|---------|---------------|-------|
| [`http_server`](http_server) | A web server with routes, using the built-in `http` module and a `blueprint` | — |
| [`json_parser`](json_parser) | `json.parse` / `json.stringify`, path queries and pretty-printing | `gdu install json` |
| [`db_connector`](db_connector) | Creating, filling and querying a SQLite database | `gdu install database` |
| [`ai_example`](ai_example) | SIMD matrix multiplication and a small neural network | `gdu install ai` |
| [`ai_example/csv_ai_training.glow`](ai_example/csv_ai_training.glow) | Training a linear model on a CSV file with the bundled `dataframe` and `glowtorch` libraries | — |
| [`flagship_showcase`](flagship_showcase) | Native modules together: JSON, BLAKE3, INT4 weights, socket polling, PNG headers | — |

## Running an example

```bash
cd json_parser
gdu install json            # only for examples that need a package
glowlang run app.glow
```

`gdu install` puts the package in `.glow_pkg/` inside the example folder, where `use "json"`
finds it.

## Installing GlowLang

* **Pre-built:** download an archive from the
  [Releases page](https://github.com/anshumali19/GlowLang-packages/releases), or run
  `gdu install glowlang`. Releases can lag behind the source.
* **From source** (newest): clone [GlowLang-core](https://github.com/anshumali19/GlowLang-core)
  and run `make` (Linux/macOS) or `.\build.bat` (Windows). The examples that use bundled
  libraries (`dataframe`, `glowtorch`, `tensor_utils`) need the `lib/` folder that comes with
  GlowLang next to the `glowlang` binary.

To build only `gdu`: `cd gdu && gcc gdu.c -o gdu -O2 -lsqlite3 -lcrypto`.

## Contributing

New examples are welcome: keep them small, make sure they run with the current build, and
describe only what the code really does. See
[CONTRIBUTING.md in GlowLang-core](https://github.com/anshumali19/GlowLang-core/blob/main/CONTRIBUTING.md).
