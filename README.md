# AI NFT Generator

## Technology Stack & Tools

- Solidity (Writing Smart Contracts & Tests)
- Javascript (React & Testing)
- [Hardhat](https://hardhat.org/) (Development Framework)
- [Ethers.js](https://docs.ethers.io/v5/) (Blockchain Interaction)
- [React.js](https://reactjs.org/) (Frontend Framework)
- [NFT.Storage](https://nft.storage/) (Connection to IPFS)
- [Hugging Face](https://huggingface.co/) (AI Models)

## Requirements For Initial Setup
- Install [NodeJS](https://nodejs.org/en/)

## Setting Up
### 1. Fork and Clone the repository 
 `git clone https://github.com/devx15/AI_NFT_Generator.git`

### 2. Setting up Node:
  1. Install node.js from the link given below:
  'https://nodejs.org/en/download'
  2. Run the the following command in CMD/Terminal
   `$ npm install`
  3. This command will download npm and all its dependencies.

### 4. Setting up the '.env' file
  '.env' file stores private tokens which are required to identify the user. Here we would be storing two tokens created from Hugging Face and NFT Storage. 
   1. Create an account on 'Huggging Face' website
       Settings                    |                     ACCESS TOKENS  
       :---------------------------------:        |      :------------------------------:
       <img src="Photos/img1.png" height="225">     |<img src="Photos/img2.png" height="225" width="180">          
    
   2. Create a personal token and copy the token in .env file in the following format 
           **REACT_APP_HUGGING_FACE_API_KEY="---Copy HERE---"
          
       NEW TOKEN                    |                    SHOW TOKENS
       :---------------------------------:        |      :------------------------------:
       <img src="Photos/img3.png" height="225">     |<img src="Photos/img4.png" height="225">          
          
          
      
   3. Create an account on NFT.Storage :
      'https://nft.storage/login/'
      <img src="Photos/img5.png" height="220" width="600">
   4. Create a personal token and copy the token in .env file in the following format 
            **REACT_APP_NFT_STORAGE_API_KEY="---Copy HERE---"**
             <img src="Photos/img6.png" height="220" width="600">

### 4. Setting up 'Hardhat'
    Hardhat is used to run and compile the solidity code. Follow these steps for setting up hardhat:
   1. Install the hardhat packages by running the following command on CMD/Terminal
   `$ npm install --save-dev hardhat`
   2. Run a test 
   `$ npx hardhat test`
   3. After successful run initiate the Hardhat Node by using the following command on CMD/Terminal
   `$ npx hardhat node`
   4. Twenty accounts and their private keys would be generated.
   5. Copy any private key from one of them.

### 5. Setting up Metamask
   1. Download and create an account on Metamask 
      'https://metamask.io/download/'
   2. After creating an account import an account by pasting the private key copied earlier.
 
       Settings                    |                     ACCESS TOKENS  
       :---------------------------------:        |      :------------------------------:
       <img src="Photos/img7.png" height="300" width="300">     |<img src="Photos/img8.png" height="300" width="500" >      
       
       
   4. Click on add network and add network manually, configure the network accordingly.
   
   <img src="Photos/Screenshot 2023-04-08 000152.png" height="400" width="300">

### 6. In a separate terminal execute:
`$ npx hardhat run ./scripts/deploy.js --network localhost`

### 7. Start frontend
`$ npm run start`
### 8. Final Step
  1. After deploying, a webpage would appear.
  2. Click on connect button.
  3. Now your setup is complete, create your NFT.......
     <img src="Photos/img9.png" height="400" width="800">
### OUR UI
Example 1                  |                   Example 2
:---------------------------------:        |      :------------------------------:
<img src="Photos/img10.jpg" height="225">  |<img src="Photos/img11.jpg" height="225">
