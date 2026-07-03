# GlowLang Examples

A curated list of official and community examples demonstrating how to build robust applications and packages in GlowLang.

*   [HTTP Server Example](./http_server)
*   [JSON Parser](./json_parser)
*   [Database Connector](./db_connector)
*   [AI / Neural Network Example](./ai_example)

---

## ⚡ Fast Installation via `gdu` (Glow Dependency Utility)
To run these examples, you need the GlowLang interpreter installed. The fastest way to install it is using `gdu`:

### 1. Download `gdu`
Download the pre-compiled `gdu` binary for your platform from the **[GitHub Releases Page](https://github.com/anshumali19/GlowLang-core/releases)**.

### 2. Run the Installer
Run the following command in your terminal to download, compile, and add the `glowlang` toolchain to your system PATH automatically:

```bash
# On Linux/macOS
gdu install glowlang

# On Windows
gdu.exe install glowlang
```

### 3. Bootstrap from Source (Alternative)
If you do not have a pre-compiled `gdu` binary, you can compile and run `gdu` manually to bootstrap the installation:

```bash
# Clone the core repository
git clone https://github.com/anshumali19/GlowLang-core.git
cd GlowLang-core/tools/gdu

# Compile gdu
gcc gdu.c -o gdu -O2 -lsqlite3

# Install the toolchain
./gdu install glowlang
```
