# How OpenSea Quickly Determines Owned NFTs  

### Events  
Solidity events, especially the `Transfer` event in ERC721 contracts, are essential for tracking the ownership of NFTs. OpenSea can set up event listeners to monitor these events and store them in an off-chain database for quick query retrieval. Even if most NFTs don’t use ERC721Enumerable, ownership data can still be accessed and processed efficiently through various methods offchain - whether in a decentralized or centralized manner. 

### Decentralized Querying  

A decentralized querying method would be The Graph.  

"Developed by Messari, the OpenSea Subgraph is a decentralized and verifiable data source for tracking and querying the Seaport marketplace protocol events on the Ethereum Blockchain.  Opensea Subgraph utilizes the Graph Protocol to extract raw blockchain data and transform it into useful metrics for effective analytics. Developers can easily retrieve data on orders, assets, and transactions that are executed on the Seaport marketplace using a unified GraphQL API endpoint."  

**Resources**:  
- [OpenSea Subgraph - Alchemy](https://www.alchemy.com/dapps/opensea-subgraph)  
- [OpenSea Subgraph - The Graph](https://thegraph.com/hosted-service/subgraph/itsjerryokolo/opensea)  

### Centralized Querying  

A centralized method to query token owners may be utilizing Alchemy's custom NFT API.  

"To get all NFTs owned by a user on a blockchain like Ethereum or Polygon, you would have to parse the entire blockchain since genesis, track all ERC-721 and ERC-1155 contracts, and track the latest ownership status of every NFT.  

This requires a massive amount of engineering resources and time.  

However, it is possible to bypass this effort by using Alchemy's NFT API."  

**Resources**:  
- [How to Get All NFTs Owned by an Address](https://docs.alchemy.com/docs/how-to-get-all-nfts-owned-by-an-address)  
