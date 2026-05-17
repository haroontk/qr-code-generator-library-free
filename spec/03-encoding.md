---
section: ISO/IEC 18004:2024 §7
status: draft
---

# 03 — Encoding

blah blah

1. **Data Analysis**
2. **Data Encoding**
3. Error Correction Coding
4. Structure Final Message
5. Module Placement in Matrix
6. Data Masking
7. Format and Version Information

## Modes

blah blah

### Extended Channel Interpretation (ECI)
- allows encoding of characters other than the default character set (mentioned below)
- ECI escape sequence is added to the data, followed by a mode indicator
- ECI is **not** supported in Micro QR Codes

### Numeric
- encodes data from the decimal digit set (0 - 9)
- Typically, 3 digits are represented by 10 bits ($2^{10} = 1024 > 999$, ie largest 3-digit number)

### Alphanumeric
- encodes data from a set of 45 characters, consisting of:
    - 10 numeric digits (0 - 9)
    - 26 alphabetic characters (A - Z)
    - 9 symbols (SPACE, $, %, *, +, -, ., /, :)
- Normally, 2 characters are represented by 11 bits ($2^{11} = 2048 > 45*45=2045$)
- $value = 45 × C_1​ + C_2​$, where $C_1$ = first character; $C_2$ = second character
- not available in M1 and M2 Micro QR Code

### Byte
- encodes 8 bits per character
- not available in M1 and M2 Micro QR Code

### Kanji
- 
- not available in M1 and M2 Micro QR Code

