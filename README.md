Building-with-Polygon-Bridge

Description
This project illustrates execution of an organization's need to move an NFT project from Ethereum to Polygon to increase demand and save on gas.

It features deployment of an NFT collection on the Ethereum blockchain, which is then mapped to Polygon, and corresponding assets transferred over via the Polygon Bridge. To put a twist to the project, the image generation tool - lexica was used to create the images for each NFT in the collection. These images were stored on IPFS using pinata.cloud and the NFT contract includes a "promptDescription" function, which when called, returns the prompt used to generate the respective image for an NFT.

The project includes a hardhat script to batch mint all NFTs (employing the ERC721A standard) and to batch transfer all NFTs from Ethereum to Polygon Mumbai using the FxPortal Bridge specifically. It first approves the NFTs to be transferred, deposits them to the Bridge, and then tests the "balanceOf" on Mumbai when state sync has happened.