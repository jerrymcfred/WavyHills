
# POLYGON HACKATHON PROJECT 2022 
## TEAM JEREMIAH (SOLO BUILD)


### PROJECT DESCRIPTION
WavyHills is a Fully Functional and fully usable NFT Marketplace for creators of fashion NFTs built using Next.js, Solidity, Polygon, TailwindCSS.
It proposes a way for innovative brands, creators, fashion photographers, Artists, Stylists, celebrities to create, buy and sell Digital clothing (for metaverse), Digital fashion, editorial photos, fashion styles, fashion photographs as NFTs.



WavyHills is made using the immense power of Solidity and Next.js. This project combines futuristic elements of Web3 blockchain development and the popular culture wave of non-fungible tokens (NFT).

This application includes creation, buying, selling and reselling of fashion NFTs and user authentication through metamask wallet. Its theme can be switched to both dark and light mode. 

Context api is used for state management and tailwind css is used for styling the application. Solidity is used to write smart contract and hardhat is used to test the smart contract.




#### How the website works
How it works;
- As a creator, to list your NFT, click on the CREATE button which shows automatically after you have connected your wallet.
- When creating your NfT, upload an image and wait for some seconds(Max-30 seconds) for it to be visible and be sure that it has been uploaded then proceed to fill in the NfT Description and price.
- Click on create and wait a little and you will prompted by METAMASK to make a payment in MATIC(Make sure you are connected on the POLYGON MUMBAI NETWORK) if everything is correct click confirm .
- After some seconds the homepage automatically refreshes and your NfT is minted and listed on WavyHills marketplace where people can purchase it.
- Once minted you will get to see all NFTs you have Minted on the Listed NfTs page.

As a Buyer;
- Click on the NFT you want to purchase and the full NFT Details page where you see details like description and others.
- To buy, click on buy button and a Modal pops up.
- Inorder for Metamask to pop up and prompt you to make payment in MATIC, you must have enough MATIC TOKENS as the listed price for the NFT. if you click on buy button and Nothing happens it means you dont have Enough MATIC tokens. (Go to https://faucet.polygon.technology/ to get free TEST MATIC TOKENS)
- Commence transfer of MATIC TOKEN AND NFT ownership becomes yours.

Note: When you Click on **CREATE** and nothing happens (Metamask doesnt pop up) after 30 seconds it means you have **Insufficient Funds** in your METAMASK WALLET and you need to get more Test matic.
###### I Suggest trying out the whole fuctionalities of WavyHills and feel a seamless flow and mind blowing User Experience. Try to create /mint NFTs, Buy NFTs, sell etc to Experience the full power of this Fashion NFT Marketplace.



#### Explanation of each page
1. **Explore NFTs** is the homepage where you get to see all NFTs listed by different sellers on WavyHills, click on each NFT to see details of the NFT.
2. **Listed NFTs** is the page where you see all NFTs that you as a creator listed on the Marketplace.
3. **My NFTs** is where you see all NFTs you have purchased on the Marketplace.





#### Not Working(You cant Mint/create NFT?)- Here are Possible Reasons
- Make sure you have Enough Test Matic Funds(the contracts are deployed on POLYGON MUMBAI NETWORK) for you to be able to create NFTs on WavyHills. 

GET TEST TOKENS HERE https://faucet.polygon.technology/

- Make sure you're connected to the POLYGON MUMBAI NETWORK on metamask.



### SUMMARY OF TECH STACK USED IN THIS BUILD;
- REACT.JS
- NEXT.JS
- SOLIDITY
- IPFS(decentralized storage)
- TAILWINDCSS
- Hardhat
- POLYGON NETWORK(MUMBAI TESTNET)
- METAMASK
- REACT CONTEXT API(state management)
- other react libraries(react-drop-zone, web3modal) etc.




### FEATURES/FUNCTIONALITIES;
- LIGHT/DARK MODE
- Seamless Fetching of data from IPFS
- Pixel perfect design
- File Uploads
- Loaders/Loading Component
- Modals
- Search/Filter functionalities
- Dynamic Routing etc




### Folder Structure
- contracts directory: this is where all smart contacts live. We already have a Migration contract that handles our migrations to the blockchain.
- node_modules directory: this is the home of all of our Node dependencies.
- src directory: this is where we'll develop our client-side application. test directory: this is where we'll write our tests for our smart contracts.
- Components directory: this is where our non pages modular components live.
- Pages directory: this is where all pages reside.
- Styles directory
- Test directory: this is where all tests for smart contracts are written.
- Context directory










## Getting Started

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!


# Installation and running the application locally

Below are instructions to get started

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, a sample script that deploys that contract, and an example of a task implementation, which simply lists the available accounts.

1. Clone the repo

```shell
git clone https://github.com/jerrymcfred/WavyHills.git
```
2. Install Packages

```shell
npm install or yarn install
```
3. Add environment variables, also you will require dedicated subdomain for IPFS from infura

```shell
API_URL= "https://polygon-mumbai.g.alchemy.com/v2/[API-KEY]"
PRIVATE_KEY = 
NEXT_PUBLIC_ALCHEMY_API_KEY = 

NEXT_PUBLIC_IPFS_PROJECT_ID = 
NEXT_PUBLIC_IPFS_API_KEY_SECRET = 
NEXT_PUBLIC_IPFS_API_HOST = "ipfs.infura.io" 
NEXT_PUBLIC_IPFS_SUBDOMAIN_NAME = 
```
4. Start the hardhat Node

```shell
npx hardhart node
```

5. In a seperate Terminal, Deploy Smart contract and make sure you update the MarketAddress in constants.js file with the new address the smart contract was deployed to

```shell
npx hardhat run scripts/deploy.js --network mumbai
```
6. Run application

```shell
npm run dev or yarn run dev
```








IMAGES;
1. When Payment is Succesful.(When Buying a listed nFTs, after buying, it reflects in the "my nfts" PAGE)
![wavy-hills vercel app_nft-details_price=0 097 tokenId=7 seller=0x2487AdEAa85d813786A876a482A88988DD4A193F owner=0x281921AA823325D606377edE0b5837b7F967FD93 image=https%3A%2F%2Fmy-music-nft infura-ipfs io%2Fipfs%2FQmShXRHM8VeXdmMBmkyvL8SeJKkp](https://user-images.githubusercontent.com/64787288/206811585-ce40511d-770d-475c-b73f-446f1cf89c9d.png)

2. When Trying to Create

![wavy-hills vercel app_create-nft](https://user-images.githubusercontent.com/64787288/206813040-b1618d56-719e-4b4f-b88d-70387e8ae60a.png)


3. The Homepage/Explore NFTS PAGE

![wavy-hills vercel app_create-nft (1)](https://user-images.githubusercontent.com/64787288/206813207-81ffe9a6-8fc4-4a09-8624-3a1d6d327314.png)
