
# ⚠️🚧 This Repo has been Archived 🚧⚠️ #

# NFT Marketplace V3

Create an NFT marketplace on top of your NFT collection on **any** EVM-compatible blockchain.

## Features

- View all NFTs from your collection and their status on the marketplace on the [buy](/pages/buy.tsx) page.

- Select which NFT from your wallet to sell for either a **direct listing** or **english auction** on the marketplace on the [sell](/pages/sell.tsx) page.

- View all NFTs a user owns from your collection on the [profile](/pages/profile/%5Baddress%5D.tsx) pages.

- Buy NFTs directly from the marketplace on the [item](/pages/token/%5BcontractAddress%5D/%5BtokenId%5D.tsx) pages.

- Place bids/offers on NFTs from the marketplace on the [item](/pages/token/%5BcontractAddress%5D/%5BtokenId%5D.tsx) pages.

<br/>

## Using this template

1. Deploy a [Marketplace V3](https://thirdweb.com/thirdweb.eth/MarketplaceV3) contract
2. Fork this repo
3. Run `yarn`
4. Plug your contract addresses, chain, highlight collection, and slideshow collections in the [contractAddresses.ts](/const/contractAddresses.ts) file.

<br/>

### Deploy the Marketplace V3 contract

Head to the [MarketplaceV3](https://thirdweb.com/thirdweb.eth/MarketplaceV3) contract page on the thirdweb dashboard.

Deploy the marketplace to the same network as your NFT collection.

<br/>

### Fork this repository

_Note: This requires [Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) and [Git](https://git-scm.com/downloads). [Yarn](https://classic.yarnpkg.com/en/docs/install/#mac-stable) is also recommended._

<br/>

### Add your contract addresses

In the [contractAddresses.ts](/const/contractAddresses.ts) file, add your contract addresses and chain.

If you haven't already, import your smart contracts into the [thirdweb dashboard](https://thirdweb.com/dashboard).

```ts
import { Sepolia } from "@thirdweb-dev/chains";
export const NETWORK = Sepolia;

// 2. The address of the marketplace V3 smart contract.
// Deploy your own: https://thirdweb.com/thirdweb.eth/MarketplaceV3
export const MARKETPLACE_ADDRESS = "0x3ccA021Ddf4a2a9c99e41Cd428Bdc44F0CebaBA6";

// // 3. The address of your Highlighted NFT collection smart contract.
export const NFT_COLLECTION_HIGHLIGHT = "0x3DFA5D25497427cB115364bd38618231378D0423";

// 4. Set up the URL of where users can view transactions on
// For example, below, we use Sepolia.etherscan to view transactions on the Sepolia testnet.
export const ETHERSCAN_URL = "https://sepolia.etherscan.io/";

// 5. Alchemy Network URL for NFT Endpoint
export const ALCH_NET = "eth-sepolia"

// 6. Your Branding
export const FOOTER_LOGO = "/zerobeings_logo_m_sepolia.png"
export const NAV_LOGO = "/zerobeings_logo_sepolia.png"
export const PROFILE_LOGO = "/user-icon.png"

// 7. Editos' choice slide show. Set the URL and the image.
// If an image link is provided, you will need to update the next.config.js with the domain. An example is provided in the next.config.js file.
export const SLIDE_1 = "0x60a8077140f4ef1d8695dfbe6869cb1ec91d1a47"
export const SLIDE_1_IMG = "https://ipfs.io/ipfs/bafybeibymtvvmsx4u5ygk5so7tumscioylkpanrthzdwhgbcqxqxsmghoa/myAuctionsToClose.png"

export const SLIDE_2 = "0x3DFA5D25497427cB115364bd38618231378D0423"
export const SLIDE_2_IMG = "/slideshow/joffee.png"

export const SLIDE_3 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_3_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png"

export const SLIDE_4 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_4_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png"

export const SLIDE_5 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_5_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png"

export const SLIDE_6 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_6_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png"

export const SLIDE_7 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_7_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png"

export const SLIDE_8 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_8_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png"

export const SLIDE_9 = "0xa0657f6290ad301ab45b703b438560d97fc2926a"
export const SLIDE_9_IMG = "https://ipfs.io/ipfs/bafybeighw4kzeqbtupjouql3rev7vlc2tit6bt55ubxvbl3235dqzdh53u/1.png" 
```
