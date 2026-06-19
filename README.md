XWaterfall
==========

XWaterfall is a fork of [Waterfall](https://github.com/PaperMC/Waterfall), which is itself
a fork of the well-known [BungeeCord](https://github.com/SpigotMC/BungeeCord) Minecraft
proxy. Upstream Waterfall has reached end of life; XWaterfall continues with our own
changes and maintenance.

XWaterfall focuses on:

- **Stability**: a testable code base and avoiding practices that lead to proxy lag.
- **Features**: more than canonical BungeeCord, plus our own additions.
- **Scalability**: handle a large number of concurrent players on modern hardware.

## How To (Server Admins)

Build a copy of `XWaterfall.jar` from source (see below). XWaterfall requires **Java 21** or above.

## How To (Compiling From Source)

To compile XWaterfall, you need a JDK (21+), git, bash, maven, and an internet connection.

```bash
git clone --recursive https://github.com/regksemx/XWaterfall.git
cd XWaterfall
./waterfall b
```

The built jar is at `Waterfall-Proxy/bootstrap/target/XWaterfall.jar`.

> This repo is patch-based: real source is the `BungeeCord/` submodule plus the
> patch series in `BungeeCord-Patches/`. Run `./waterfall` with no arguments to
> see the available patch and build commands.

## Credits

Built on the work of [PaperMC/Waterfall](https://github.com/PaperMC/Waterfall) and
[SpigotMC/BungeeCord](https://github.com/SpigotMC/BungeeCord).
