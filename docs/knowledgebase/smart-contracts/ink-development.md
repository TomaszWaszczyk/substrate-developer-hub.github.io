---
title: ink! Development
---

ink! is a [Rust](https://www.rust-lang.org/)-based embedded domain specific language
([eDSL](https://wiki.haskell.org/Embedded_domain_specific_language)) for writing
[WebAssembly](https://webassembly.org/) smart contracts specifically for the
[FRAME Contracts pallet](contracts-pallet).

ink! is still under development, so the documentation for using it is sparse. However, on this page
you will find the best resources to get you started building ink! contracts right away.

## Tutorials

The ink! project maintains an up-to-date tutorial teaching all the basics of developing on ink!.

**This is the best way to get start learning the language today.**

<a class="btn btn-secondary primary-color text-white"
href="https://substrate.dev/substrate-contracts-workshop/">Start the ink! tutorial!</a>

You will learn how to:

- Set up your computer to build and deploy ink! smart contracts.
- Learn the basics of ink! by creating an incrementer contract.
- Learn more advance tricks by developing an ERC20 contract.

## Example Contracts

ink! provides a
[set of example smart contracts](https://github.com/paritytech/ink/tree/master/examples) that can
help you understand how it is similar and different to other smart contract languages.

This includes:

- [A Flipper Contract](https://github.com/paritytech/ink/tree/master/examples/flipper/)
- [An ERC20 Contract](https://github.com/paritytech/ink/tree/master/examples/erc20/)
- [An ERC721 Contract](https://github.com/paritytech/ink/tree/master/examples/erc721/)
- [A Delegator Contract](https://github.com/paritytech/ink/tree/master/examples/delegator/)

## FAQ

Here are some answers to frequently asked questions developers have while building on ink!.

### What is the difference between memory and storage?

In ink!, `memory` refers to computer memory, while `storage` refers to the on-chain storage used by
a contract instance. `memory` is temporary and only lasts until the contract execution is done,
while `storage` is persistent and lasts over many contract executions. The contract `storage` is
built on top of the runtime storage, and access is considered to be slow.

### How do I run tests?

When building a smart contract with ink!, you can define a set of tests.

For example, in the minimal
[flipper contract](https://github.com/paritytech/ink/blob/master/examples/flipper/lib.rs), you
can find a small test at the bottom of the contract.

You should run this test just like you would any other Rust test:

```bash
cargo +nightly test
```

## Get Help

Join the growing community of ink! smart contract developers:

- Ask development questions on [StackOverflow](https://stackoverflow.com/questions/tagged/ink) with
  the `ink` tag.
- Join the live chat in the
  [Smart Contracts & Parity ink!](https://riot.im/app/#/room/!tYUCYdSvSYPMjWNDDD:matrix.parity.io)
  on Riot.
- Report bugs, make feature requests, and ask technical questions on the
  [ink! GitHub](https://github.com/paritytech/ink).

## Next Steps

### Learn More

- Learn more about the design philosophy of
  [ink! in our conceptual documentation](ink-fundamentals).
- Learn more about the [Contracts pallet](https://substrate.dev/rustdocs/v3.0.0/pallet_contracts/index.html).

### Examples

- Follow a
  [tutorial to add this Contracts pallet to your Substrate runtime](../../tutorials/add-contracts-pallet/).

### References

- Visit the
  [ink! repository for additional docs and to look at the source](https://github.com/paritytech/ink).
- Visit the [ink! developer homepage](https://paritytech.github.io/ink/)
- Visit the reference docs for the [ink! metadata](https://paritytech.github.io/ink/ink_metadata/).
- Visit the reference docs for the [core ink! language](https://paritytech.github.io/ink/ink_lang/).
