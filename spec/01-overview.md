---
section: ISO/IEC 18004:2024 §
status: draft
---

# 01 — __ overview


## What is QR Code?

QR Code is a 2D matrix of square **modules** arranged in an overall square pattern to represent some data.

It must have the following characteristics:
1. Be in the format of QR Code or micro QR Code
2. Have an encodable character set, such as numeric, alphanumeric, binary and kanji
3. Represent data obviously
4. Be in the form of a matrix
5. Be usable rotated or reflected

For QR Codes:
- version reference is in the form V-E, where V identifies the version number (1 to 40) and E indicates error correction level (L, M, Q or H)
- symbol size must be between 21 x 21 modules and 177 x 177 modules (1 to 40, increasing in steps of 4 modules on each side)
- maximum characters in a symbol(version 40-L) is 
 - 7089 : numeric
 - 4296 : alphanumeric
 - 2953 : byte
 - 1817 : kanji

For micro QR Codes:
- version reference is in the form MV-E, where M indicates micro QR Code, V identifies the version number (1 to 4) and E indicates error correction level (L, M or Q)
- symbol size must be between 11 x 11 modules and 17 x 17 modules (M1 to M4, increasing in steps of 2 modules on each side)
- maximum characters in a symbol(version M4-L) is 
 - 35 : numeric
 - 21 : alphanumeric
 - 15 : byte
 - 9 : kanji

**modules** - 