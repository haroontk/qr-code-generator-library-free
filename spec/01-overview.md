---
section: ISO/IEC 18004:2024 §
status: draft
---

# 01 — overview


## What is QR Code?

QR Code is a 2D matrix of square **modules** arranged in an overall square pattern to represent some data.

It must have the following characteristics:
1. Be in the format of QR Code or micro QR Code
2. Have an encodable character set, such as numeric, alphanumeric, binary and kanji
3. Represent data
4. Be in the form of a matrix
5. Have orientation independence, including rotation and reflection

For QR Codes:
- version reference is in the form V-E, where V identifies the version number (1 to 40) and E indicates **error correction level** (L, M, Q or H)
- symbol size must be between 21 x 21 modules and 177 x 177 modules (1 to 40, increasing in steps of 4 modules on each side)
- maximum characters in a symbol(version 40-L) is 
 - 7089 : numeric
 - 4296 : alphanumeric
 - 2953 : byte
 - 1817 : kanji

For micro QR Codes:
- version reference is in the form MV-E, where M indicates micro QR Code, V identifies the version number (1 to 4) and E indicates **error correction level** (L, M or Q)
- symbol size must be between 11 x 11 modules and 17 x 17 modules (M1 to M4, increasing in steps of 2 modules on each side)
- maximum characters in a symbol(version M4-L) is 
 - 35 : numeric
 - 21 : alphanumeric
 - 15 : byte
 - 9 : kanji


**OPTIONAL** features:
- **Structured Append** : allow files to be 
- Allow use of other character sets or data interpretations
- Allow colours to be swapped (light on dark background)
- Allow to be produced in a mirrored form


> **NOTE**: The difference between *reflection in orientation independence* in mandatory characteristics and *Allow to be produced in a mirrored form* in optional features is that the former specifies that a QR Code must have structural information that allows the decoder to infer its orientation and do the necessary adjustments to be able to decode it, while the latter specifies the ability for an encoder to create mirrored QR Codes.



**Modules** - smallest pixel that makes up the matrix

**Error Correction Level** : levels of Reed-Solomon error correction, allowing recovery of data upto :
 - L : 7%
 - M : 15%
 - Q : 25%
 - H : 30%