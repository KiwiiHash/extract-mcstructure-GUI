# extract-mcstructure

A tool for extracting `.mcstructure` files from a Minecraft Bedrock world’s LevelDB database.  
These structures may include ones saved using the `/structure` command. The extracted `.mcstructure` files can then be imported into other worlds.

---

## Usage

### Example extract all structures

```bash
python3 run.py World all
````

Extracts **all `.mcstructure` files** from the world named `World` (the name shown in the in-game world list).

---

### Extract a specific structure & Specify output directory

```bash
python3 run.py World house -o example/output
```

Extracts the structure named `house` from the world `World` and saves it to the directory named output:

```
example/output
```

---

### Output directory

Use the `-o` flag to specify where extracted files should be saved.

If not specified, the program will use its default output location.

---

## GUI Mode (Unstable)

You can launch the graphical interface with:

```bash
python3 beta.py
```

> The GUI mode is experimental and mainly intended for **Linux users**. *(Using Wine)*

---

## Why use this?

Some versions of **Minecraft Bedrock Edition** do not include the built-in **Export** button for structures.

This tool allows you to manually extract `.mcstructure` files from a world, making it possible to:

* Recover structures from worlds
* Transfer structures between worlds
* Export structures on devices where the export feature is unavailable

---

## Dependencies / Credits

* `leveldb` library from
  [https://github.com/Amulet-Team/Amulet-Core](https://github.com/Amulet-Team/Amulet-Core)

* `tkinter` (used by `beta.py`) — included with Python

* `Termux` Android app
  [https://github.com/termux/termux-app](https://github.com/termux/termux-app)
