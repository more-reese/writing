Published with [PubDAO](https://pubdao.co/) on [Decrcypt](https://decrypt.co/resources/what-is-erc-1155-ethereums-flexible-token-standard), June 2022

# What is ERC-1155? Ethereum's Flexible Token Standard
### ERC-1155 is a token standard that enables the efficient transfer of fungible and non-fungible tokens in a single transaction.

Everything that happens on Ethereum, at the most fundamental level, is represented by data. Whether you swap ETH for USDC on Uniswap or buy a CryptoPunk on OpenSea, everything included in the transaction—your wallet address, fungible tokens, non-fungible tokens, decentralized applications, etc.—is broken down into smaller, computer-readable chunks of data. 

For a transaction to be considered legitimate, its data must be shared across the network, validated, and processed by computers that then store the transaction data in a block. A transaction's size and complexity determines the cost and time required to process it.

In the same way that not all transactions are created equal, not all tokens on Ethereum are created equal. Some tokens are generic and easily interchangeable (for example, UNI, COMP and GRT) while others are unique (for example, non-fungible tokens or NFTs). As such, different token standards exist to address different use cases.

This article discusses ERC-1155, a flexible Ethereum token standard that allows for the transfer of multiple types of token at once.

## What is ERC-1155?
All updates to Ethereum go through the Ethereum Improvement Proposal (EIP) process. Anyone from the community can submit a proposal. If it meets certain standards, it becomes an EIP which is then discussed and voted on. If the proposal passes, Ethereum is updated with its improvements.

"ERC" stands for Ethereum Request for Comments. It is a type of EIP focused on standards for Ethereum applications, a category that includes tokens. 

Tokens are transferable units of value. Colloquially they are referred to as cryptocurrencies or (technically incorrectly) coins. Tokens generally fall into one of two buckets: fungible or non-fungible. Fungible tokens are mutually interchangeable, like dollar bills or pesos. Non-fungible tokens are unique and noninterchangeable, like a painting or book.

Prior to ERC-1155, the two predominant token standards were ERC-20 for fungible tokens and ERC-721 for non-fungible tokens. They could not (and cannot) be wrapped into the same smart contract. This limitation meant that if someone wanted to transfer, say, USDC (ERC-20) and a CryptoKitties NFT (ERC-721), they would need to execute multiple transactions, which was inefficient and expensive.

ERC-1155 solves for this by combining the two token standards. ERC-1155 is a token standard that enables the efficient transfer of fungible and non-fungible tokens in a single transaction. Witek Radomski, Andrew Cooke, Philippe Castonguay, James Therien, Eric Binet, and Ronan Sandford proposed the new standard in June 2018 with EIP-1155.

## How does ERC-1155 work?
The initial motivation behind ERC-1155 was to address challenges faced by blockchain game developers and players. There are plenty of examples of ERC-1155 being used outside of gaming. However, gaming is a great reference use case for understanding how ERC-1155 works.

Massively multiplayer online games (MMOs) contain tens of thousands of items—armor, weapons, shields, skins, coins, badges, castles, etc—that players can collect and trade with one another. Some items like coins are fungible while others like a sword are non-fungible. On the blockchain, each one of these items is a token.

Prior to ERC-1155, each item required its own smart contract. In a game with 100,000 items that means 100,000 smart contracts! As ERC-1155 developer Witek Radomski pointed out, that's like needing a different phone for each app you use. It creates lots of unnecessary redundancy and is an inefficient use of space and money.

With an ERC-1155 token, multiple items can be stored in a single smart contract and any number of items can be sent in a single transaction to one or more recipients. This means if you wanted to send a sword to one friend, a shield to another, and 100 gold coins to both, you could do so in only one transaction. 

If you're interested in understanding how ERC-1155 works at a technical level, check out EIP-1155.

## What's so special about ERC-1155?
As well as allowing for the transfer of multiple token types at once, and the attendant gains in efficiency and lower transaction costs, ERC-1155 has a number of other special characteristics:

- It supports an infinite number of tokens, in contrast with ERC-20 and ERC-721, which require a new smart contract for each type of token.
- It supports not only fungible and non-fungible tokens, but also semi-fungible tokens. Semi-fungible tokens are like general admission concert tickets. - They are interchangeable and can be sold for money before the show (fungible). But after the show they lose their pre-show value and become collectibles (non-fungible).
- It has a safe transfer function that allows tokens to be reclaimed if they are sent to the wrong address, unlike ERC-20 and ERC-1155.
- It removes the need to "approve" individual token contracts separately, which means signing fewer transactions.

## Who's using ERC-1155?
- 🎮 Enjin - Enjin offers a number of blockchain products, many of which implement ERC-1155.
- 🕹️ Horizon - Horizon is a blockchain games company whose Skyweaver game uses ERC-1155.
- 🖼️ OpenSea - The NFT marketplace's ERC-1155 implementation allows multiple creators per smart contract but only one creator is able to mint more copies. 
- 🎈 OpenZeppelin - OpenZeppelin's blockchain security products leverage the ERC-1155 standard.

## The future of ERC-1155
Although ERC-1155 has been around for four years, it is still relatively underutilized compared to its ERC-20 and ERC-721 counterparts. This may come as a surprise given ERC-1155's versatility; it’s possible that existing non-ERC-1155 projects will migrate to the new standard in order to expand their functionality.

ERC-1155 will continue to be used in blockchain games built on Ethereum. The advent of play-to-earn games could expedite this process.
