# Setting Up an Environment

Will need to know Rust.

I am reading the Rust Book currently. Need to continue reading!

Dependencies:

Rust compiler
Wasm package

-

We need wasm binaries:

`rustup target add wasm32-unknown-unknown` is the target

We need to check to ensure that contracts are correct and ready to be uploaded to the chain:

`cargo install --features iterator` <-- wait... not anymore.

`cargo install cosmwasm-check` <-- current package

First we need some smart contract examples

- cloned cw-plus repo

-- so now I have two repos related to this class
    -- cw-plus (cloned from https://github.com/CosmWasm/cw-plus)
    -- cw-academy (created on my personal github account)

- cw-plus repository

- ran this command: `cosmwasm-check ./target/wasm32-unknown-unknown/release/cw1_whitelist.wasm`

- we can run `cosmwasm-check` on wasm contracts to generate a test to see if the contracts work.

- I ran that on the cw-whitelist that I cloned from the cw-plus repo, and the check passed.

That's the end of the first lesson!
