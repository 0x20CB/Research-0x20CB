# Liberatø: Addressing Scheme For Decentralized Entities Using Blake2s and Blake2b

## Preface

Written by 0x20CB (Joseph P. Tortorelli)

## Liberato Addressing Scheme

To create the addressing scheme, we use the hash function `blake2s` and `blake2b` to create digests of variable length, which is then encoded in hexadecimal.

The variable digest gives us around `40 address spaces`

That would be from 192-512 bits, assumed to be secure enough.

Due to Blake2b's nature of variable hashing, we can create different hashes from same inputs.

### Assigning Source

To assign the `source` of the parser, we use `X59-fmt`.
