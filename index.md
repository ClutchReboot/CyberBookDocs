## Purpose
This is a collection of functions / tools that are used frequently enough to store them some place.

### DecoderRing Example
The purpose of DecoderRing is to encode / decode a string easily.
```python
import CyberBook

# DecoderRing Usage
dr = CyberBook.DecoderRing(data='test')

print(
    # Encode using Hex
    f"Hex encoded: \t\t{dr.hex()}",

    # Encode using Base64
    f"Base64 encoded: \t{dr.base64()}",

    # Access data and altered_data
    f"Initial input: \t\t{dr.data}",
    f"Encrypted string: \t{dr.altered_data}",

    # Decode Base64
    f"Base64 decoded: \t{dr.base64(decode=True)}",

    # Decode Hex
    f"Hex decoded: \t\t{dr.hex(decode=True)}",
    sep='\n'
)
```
Expected Output:
```commandline
Hex encoded: 		74657374
Base64 encoded: 	NzQ2NTczNzQ=
Initial input: 		test
Encrypted string: 	NzQ2NTczNzQ=
Base64 decoded: 	74657374
Hex decoded: 		test
```