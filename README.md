# 📝 Kirby's Adventure Disassembly Notes

Welcome to my reverse-engineering exploration of **Kirby’s Adventure** (NES).  
Here we dig deep into the 6502 assembly, graphics, and level data. ⚡

---

## 🛠 Tools Used

- **NESGodisasm** – Disassembly of the ROM
- **YY-CHR** - The .chr file

---

## 🔹 Key Findings

### Code Entry Points
- `$8000` – Start of PRG-ROM
- `$C000` – Interrupt vectors
- `$9000-$BFFF` – Main game loop

### Graphics & Sprites
- Tile format: **2bpp, NES 8x8 tiles**
- Sprite RAM: `$0200-$02FF`  
- Palette memory: `$3F00-$3F1F`

### Levels
- Stored as compressed arrays in PRG-ROM
- Each byte represents a block or enemy spawn

---

## 🖼 Screenshots & Diagrams

### Tile Example
![Tile Example](https://via.placeholder.com/150x150.png?text=Kirby+Tile)

### Memory Map Sketch
$0000-$07FF: RAM
$2000-$2007: PPU registers
$4000-$401F: APU / I/O
$8000-$FFFF: PRG-ROM


## 💡 Notes & TODOs

- [ ] Document all enemy routines
- [ ] Identify unused tiles & clean up
- [ ] Map full level layouts
- [ ] Add custom textures & test modifications

---

## 📖 References

- NESDev Wiki – [https://www.nesdev.org](https://www.nesdev.org)  
- FCEUX Debugging Guide  
- Original Kirby’s Adventure ROM

---

Made with ❤️ by a retro-hacker 🕹
