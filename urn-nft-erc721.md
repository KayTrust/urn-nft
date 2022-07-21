# Unique resource name (URN) format for ERC721 Non-Fungible Tokens

# Introduction

This document describes a globally unique identifier format for ERC721 NFTs, extending the `urn:nft` namespace.

# What is ERC721?

TODO: Briefly recap how ERC721 works: what Ethereum is, how smart contracts are used, how tokens are identified, etc.

# Schema

The URN format for ERC721 NFTs extends the [`urn:nft` namespace](urn-nft.md). The specific format is the following:

`urn:nft:erc721:<chain_id>:<contract_address>:<token_id>`

where:
- `<chain_id>` is the Ethereum ChainID. While technically two different blockchain can use the same ChainID, it is assumed that the ChainID be unique between all actors that refer to an ERC721 NFT URI. How clashes are avoided is a general discussion about ChainID and is outside the scope of this document.
- `<contract_address>` is the Ethereum smart contract address deployed on the blockchain with the specified chain_id.
- `<token_id>` is the TokenID as defined by the ERC721 specification.
