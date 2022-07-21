# URN namespace for Non-Fungible Tokens

## Introduction

Non-fungible tokens (NFTs) are objects with an identifier whose uniqueness is enforced by a blockchain. Additionally, each NFT also has specific metadata, also defined on its host blockchain, the most important of which is its owner.

The unique identifier of a non-fungible token, known as Token ID, is only unique within the smart contract where it is defined, but not globally unique. For applications that refer to the NFT within a smart contract, a locally unique identifier is sufficient. However, other applications sometimes need to refer to NFTs globally. This document is an attempt to map local Token IDs to more global identifier through the definition of a new URN namespace for NFTs.

## Namespace

The proposed namespace is `urn:nft`. The syntax is the following:
 `urn:nft:<nft_method>:<method_specific_identifier>`

The `<nft_method>` component is the unique identifier for an NFT algorithm. A registry shall be maintained to define well-known NFT methods.

Each NFT method shall be defined within its own specification, and must detail how the `<method_specific_identifier>` is used to point to a specific NFT created using that method.