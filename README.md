# Nes
A emulator for **NES (Nintendo Entertainiment System)** made in Rust capable of run games like:  
	- **PacMan  
	- Donkey Kong  
    	- Super Mario Bros  
    	- etc.**  

---

# Installation

In Debian-based distros, run:
```sh
sudo apt install git cargo
git clone https://github.com/DevAles/nes.git
cd nes
chmod +x ./debian-install
./debian-install
```

In Arch-based distros, run:
```sh
yay -S git rust
git clone https://github.com/DevAles/nes.git
cd nes
chmod +x ./arch-install
./arch-install
```

---

# Running

```sh
chmod +x ./start
./start
```

---

# Credits

This emulator was built following [nes_ebook](https://github.com/bugzmanov/nes_ebook) by [@bugzmanov](https://github.com/bugzmanov) — the CPU, PPU, bus, cartridge and render implementations are adapted from the `code/ch8` chapter of that book.

Things added on top of the book's code:  
	- Code restructured into `lib.rs` + `components/` modules  
	- Game selection through stdin  
	- Frame pacing with `fps_clock`  
	- Install scripts for Debian and Arch based distros

---

# References

Some useful links that i use to build this emulator:  
	- [6502 Instruction Reference](https://web.archive.org/web/20210428044647/http://www.obelisk.me.uk/6502/reference.html)  
	- [6502 Assembly Reference](https://en.wikibooks.org/wiki/6502_Assembly)
