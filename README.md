# Nano96

Nano96 is my own custom 96% ANSI mechanical keyboard, designed from scratch. And with everyone's first hardware project (assuming), it was a crazy experience. I had a giant DRC battle (209 errors!!!), a footprint swap that caused courtyard collisions across the whole board, a near-disaster where a folder overwrite almost wiped two days of LED work, and a jumpscare where I thought I'd lost my routing entirely after accidentally force-closing Freerouting. All of that is documented in the journal.

The board has 97 hotswappable switches, 99 individually-addressable per-key RGB LEDs (reverse-mounted so they shine up through the plate), a 0.91" OLED display, and an I2C rotary encoder with a push-button. It's wireless, built around a nice!nano v2 (nRF52840) running ZMK, with an MCP23017 I2C expander handling the extra GPIO the matrix needed.

The case is 3D-printed in PETG — black body with red accents — using a gasket-mount design (foam-cushioned plate, sandwiched between a bottom tray and a top rim), with a USB-C cutout and a Poron foam floor for acoustic dampening.

I wanted to make this because I am in a very bad need for a keyboard, and this is it!
(i can also get it for free, lol)
## CAD renders

(wip!)

## BOM
<img width="1179" height="651" alt="Screenshot 2026-08-24 at 8 51 59 AM" src="https://github.com/user-attachments/assets/c05f3bf6-3b38-4c06-9c0e-44f347549f8b" />


## v2 ideas
  
- Considered a color OLED upgrade (full color GIFs would be heaven, i could also run Doom on it, lol) but the interface change (I2C to SPI) and cloudy ZMK driver support made it too risky to attempt this close to the deadline. So it's going in my v2.
- Ground plane / copper pour was attempted but reverted before submission — landed inside the nice!nano's antenna keepout zone and needs to be redone carefully in v2. 
- Kickstand feet were prototyped in an earlier case revision but dropped when switching to gasket mount.

## License

*(add your preferred license)*
