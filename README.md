# PiFS (Pi File System / Cipher)

A steganographic coordinate-pointer cipher that turns the digits of $\pi$ into a shared reference book. Instead of transmitting raw text, it encodes messages into compressed delta-encoded byte streams pointing to absolute offsets inside a local copy of $\pi$.

## Project Structure
- `pi_digits.txt`: The local database (10 million digits of $\pi$).
- `pifs`: The core CLI script.

## Usage

Make the script executable:
```bash
chmod +x pifs
```
Encoding:

```bash
python3 pifs -e "String to be encoded."
```
Decoding:

```bash
python3 pifs -d "Output of a previously encoded string."
```
