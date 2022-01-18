Package created to simplify the process of parsing NFTs on Solana.

It consists of:

Package basic things like fetch all NFTs for specific wallet. Designed to be used in browser or Node.JS env.

Soon:
For react - bunch of hooks and utils to be used within React app.

# How to use

`getParsedNftAccountsByOwner` - return parsed list of NFTs (SPL Tokens) for given wallet public address. Each item in array have all data specified on the blockchain. The NFT metadata stored separately, you need to pick uri property for each token and fetch data youself.

` import {                                        `
`  getParsedNftAccountsByOwner                    `
`} from "@nfteyez/sol-rayz";                      `
`                                                 `
`const tokenList = getParsedNftAccountsByOwner(); `

`createConnectionConfig` - method for creating a "connection" with Solana, have two params: clusterApi and commitment.

`getParsedNftAccountsByOwner` - method to get array of parsed NFTs by owner address. Have three params: wallet address(required), connection , serialization (true/false).

`isValidSolanaAddress` - check if provided string is valid Solana address.
