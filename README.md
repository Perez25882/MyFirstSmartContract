This is my first attempt at writing a smart contract using Solidity as part of Lesson 1.3 of the Solidity Programming 101 course. Below, I’ve documented the process I followed to set up the environment, write the code, compile, deploy the contract, and push everything to GitHub.

Part 1: Setting Up the Development Environment
1. MetaMask Setup
I started by installing the MetaMask browser extension.
I created an Ethereum wallet and carefully stored the seed phrase (I’ll probably never remember it if I lose it).
2. Accessing Remix IDE
I opened Remix IDE in my browser and created a new workspace called MyFirstSmartContract.
Then, I added a new Solidity file named SimpleStorage.sol where I planned to write my first smart contract.

Part 2: Writing the Smart Contract
Here’s the code I wrote for the contract:

// SPDX-License-Identifier: MIT  
pragma solidity ^0.8.25;

contract SimpleStorage {
    uint256 favoriteNumber;

}
This contract is pretty simple:
It has a variable called favoriteNumber (of type uint256), which stores a number.

Part 3: Compiling and Deploying the Contract
1. Compiling the Code
In Remix, I went to the Solidity Compiler tab and made sure the version was ^0.8.25.
I clicked Compile to make sure there were no issues (thankfully, there were none).
2. Deploying Locally
Under the Deploy & Run Transactions tab, I selected Remix VM (Cancun) as the environment.
I deployed the SimpleStorage contract to the local blockchain.

Part 4: Pushing to GitHub
1. Connecting Remix with GitHub
I connected Remix to my GitHub account (following some instructions I found).
I created a public GitHub repository named MyFirstSmartContract.
I added this repository as a remote inside Remix.
2. Committing and Pushing the Code
Finally, I pushed the SimpleStorage.sol file to the repository directly from Remix.

Part 5: Challenges and How I Overcame Them
Browser Issues with MetaMask:

At first, MetaMask didn’t work on my default browser, so I switched to Chrome, and it worked fine.
Compiler Version Mismatch:

I forgot to check the compiler version in Remix, and it threw an error. Once I selected version 0.8.25, everything compiled smoothly.
GitHub Authentication Problem:

I had some trouble with GitHub because of two-factor authentication. I ended up generating a personal access token to log in instead of using my password.
Conclusion
This was a fun and eye-opening experience! It felt great to go from installing MetaMask to writing and deploying my very first Solidity contract. Now that it’s pushed to GitHub, I’m excited to learn more and try more advanced smart contracts in the future.

