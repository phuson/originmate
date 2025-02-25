# Originmate

A library of module building blocks for Move on Sui.

Movemate provides an advanced standard library of common modules in the Move ecosystem (working in tandem with the native frameworks), focusing on security, efficiency, composability, and ease of implementation.

Forked from: [pentagonxyz/movemate](https://github.com/pentagonxyz/movemate)

## Modules

- `acl`: Multi-role access control list (ACL).
- `bcd`: Binary canonical Deserialization. Convert `vector<u8>` to `u64` and `u128`.
- `bloom_filter`: Space-efficient probabilistic data structure for checking if an element is part of a set.
- `box`: Transfer objects with the `store` ability but not the `key` ability.
- `crit_bit`: [Crit-bit trees](https://cr.yp.to/critbit.html) data structure. (Thanks to Econia.)
- `crit_bit_u64`: [Crit-bit trees](https://cr.yp.to/critbit.html) data structure. (Thanks to Econia.) Uses `u64` keys.
- `date`: Date conversion library in Move.
- `escrow`: Basic object escrow module on Sui.
- `escrow_shared`: Basic object escrow module with refunds and arbitration on Sui.
- `governance`: On-chain coinholder governance (store coins and other objects).
- `i64`: Signed 64-bit integers.
- `i128`: Signed 128-bit integers.
- `linear_vesting`: Linear vesting of coins for a given beneficiary.
- `math`: Standard math utilities missing in the Move language (for `u64`).
- `math_safe_precise`: `mul_div` for `u64`s while avoiding overflow and a more precise `quadratic` function.
- `math_u128`: Standard math utilities missing in the Move language (for `u128`).
- `merkle_proof`: Merkle proof verification utilities.
- `pseudorandom`: Pseudorandom number generator.
- `to_string`: `u128` to `String` conversion utilities.
- `vectors`: Vector utilities--specifically, comparison operators and a binary search function.
- `virtual_block`: Replace latency auctions with gas auctions (with control over MEV rewards) via virtual blocks.

## Publishing

```
sui client publish --path ./movemate/sui --gas-budget 30000
```
