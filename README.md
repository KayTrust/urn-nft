# Unique URIs for Non-Fungible Tokens (NFTs)

This repository describes a method to refer to NFTs through globally unique URIs, based on [RFC 8141: Uniform Resource Names (URNs)](https://datatracker.ietf.org/doc/html/rfc8141).

It is structured in the following way:
- [urn-nft.md](urn-nft.md) defines the main `urn:nft` syntax
- Method-specific documents describe how NFTs should be identified for each well-known NFT framework, e.g. ERC-721.

# Known methods

This section lists known NFT methods. It could be maintained as a separate document in the future, if needed.

| NFT Method | Description | Specification
|------------|-------------|--------------
| `erc721`   | ERC-721 NFTs (based on Ethereum) | [`urn:nfc:erc721` specification](urn-nft-erc721.md)
