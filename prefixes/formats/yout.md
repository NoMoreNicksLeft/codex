# ID format description

Youtube video IDs (and Channel IDs) use a modified form of base64 encoding to encode 64 bit integers (and 128 bit ints). Those are plain numbers, basically, though large ones. The modifications substitute "-" (dash) and "_" (underscore) for the slash and plus that base64 usually uses... likely because those are used for other things in URLs. Because of the size of the underlying numbers, the encoded versions will probably always be 11 characters (and 22 characters) long. However, Google makes no promises that this will be the case into the indefinite future.

    kFpYU43QU4c

It is embedded in the URL, like so:

    https://www.youtube.com/watch?v=kFpYU43QU4c

There are issues with using the encoded version (non-number) in filenames. For some filesystems, they make no distinction between k and K (lower and uppercase), but these are two distinct IDs. See this Stack Exchange answer for a more thorough explanation:

https://webapps.stackexchange.com/a/54448/253000

The shortest encoding might be hexadecimal And it might be advisable to use big-endian for that hexadecimal as well (read the above answer).

Some tool or script one-liner would need to be developed to convert these back and forth, if anyone intends to use this format.
