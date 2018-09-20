# HASH FUNCTIONS
Introduction to the concept of hash functions

A cryptographic hash (sometimes called ‘digest’) is a kind of ‘signature’ for a text or a data file. SHA-256 generates an almost-unique 256-bit (32-byte) signature for a text.

A hash is not ‘encryption’ – it cannot be decrypted back to the original text (it is a ‘one-way’ cryptographic function, and is a fixed size for any size of source text). This makes it suitable when it is appropriate to compare ‘hashed’ versions of texts, as opposed to decrypting the text to obtain the original version.

This script is oriented toward hashing text messages rather than binary data. The standard considers hashing byte-stream (or bit-stream) messages only. Text which contains (multi-byte) characters outside ISO 8859-1 (i.e. accented characters outside Latin-1 or non-European character sets – anything with Unicode code-point above U+FF), can’t be encoded 4-per-word, so the script defaults to encoding the text as UTF-8 before hashing it.

Note that what is returned is the textual hexadecimal representation of the binary hash. This can be useful for instance for storing hashed passwords, but if you want to use the hash as a key to an encryption routine, for example, you will want to use the binary value not this textual representation.

For more details in this [link](https://www.movable-type.co.uk/scripts/sha256.html)
