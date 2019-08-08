# Procedural Map Generator

A small toy project written in Rust: procedural generation of 2D grid-based maps with simple terminal-based visualisations


* ``Pipe graphs`` - an interconnected network of pipes/roads/subways/hallways or whatever you see in it.
    * No isolated subgraphs.
    * Two classes of pipes, a 'backbone' or set of core pipes (thicker) vs 'regular'
    * Simple visualisation (using unicode block drawing) to standard output
* ``Height graphs`` - Each cell has a height, good for landscapes

![Screenshot](https://raw.githubusercontent.com/proycon/procmapgen/master/screenshot.png)

## Build instructions

Assumes you have Rust and Cargo installed:

```
$ git clone https://github.com/proycon/procmapgen
$ cd procmapgen
$ cargo build --release
```

Usage:

```
$ ./target/release/procmapgen --help
```

It's fun to use this with ``watch`` to random ones continuously:

```
$ watch -n 0.5 ./target/release/procmapgen
```
