- Instead of `create-reacr-app` we will be using `vite`
- npm init vite@latest
- npm run dev

# Now we will setup `tailwind-css` 
-  npm install -D tailwindcss postcss autoprefixe 
- npx tailwindcss init -p
  now follow below link for further 
 https://tailwindcss.com/docs/guides/create-react-app

 ## cd smart_contract 
 - npm init -y

 ## cd client `installing extra packages` 
 - npm install react-icons
 - npm install react-icons ethers

 <hr>

 on `index.css` change `eh-card` to `polygon` for `welcome` page 

 <hr>

 Go to `Loader` and change the `Loader` as you wish for `welcome page` 

<hr>

# cd `smart_contract`
`commands`

- `npx hardhat`

- npm install --save-dev "hardhat@^2.8.0"

- npm install --save-dev "hardhat@^2.13.0" "@nomicfoundation/hardhat-toolbox@^2.0.0"

- npx hardhat compile

- npx hardhat test

- `Also refer below site`
`https://hardhat.org/hardhat-runner/docs/getting-started#overview`

- also get `solidity extension` in vs code 

# Info about `Hardhat`
- `hartdhat` is a etherium development enviroment for developers ,we need to use `polygon` chain 
- It allows us to run `solidity` locally


# Important about ethereum address , wallet transffer

- use below given site and connect your wallet 

`https://faucet.quicknode.com/ethereum?utm_term=eth%20faucet&utm_campaign=Product+%7C+Faucet&utm_source=google&utm_medium=cpc&hsa_acc=1365030395&hsa_cam=18518073344&hsa_grp=145076429467&hsa_ad=626347581499&hsa_src=g&hsa_tgt=kwd-321228529343&hsa_kw=eth%20faucet&hsa_mt=b&hsa_net=adwords&hsa_ver=3&gclid=CjwKCAjw_YShBhAiEiwAMomsEFf1KkyOJPk91G654L57unOQVD8x8eZ4hDGZ6B5hwN6IP60rra88gBoCsewQAvD_BwE` 

<hr>

# sites to visit and study
- `hardhat-waffle`
- `developers.giphy.com` 

<hr>

# Deployment process
- got to `alchemy.com` and select `start for free`

- make changes in the `hardhat.config.js` file and run the below command
 `npx hardhat run scripts/deploy.js --network mumbai`
          or for ethereum addres use below
 `npx hardhat run scripts/deploy.js --network goerli`
 - after compilation it will provide us `Transaction address` 
 - it will look like : `Transactions address:  0x9195aE8EB0e3819bFb0ae0dd6E111f62EA1fE27f`

 <hr>

 ## here is what we need to change from etherium to polygon 
 - In ` src/transactionCOntext.js` change `{ethers}` to {polygon} its a object 


  Open metamask and choose Rinkeby Test Network
- Get some ETH from rinkeby faucet for your account
- Create the App on Alchemy choosing - Chain: Ethereum, Network: Rinkeby
- Copy HTTP key of this app
- Define rinkeby (INSTEAD of ropsten) in networks in hardhat.config.js (just like in the video)
- Paste the HTTP key in url (follow the video too)
- Take the private key from your account, paste into accounts (make sure, you are in rinkeby test network)
- Deploy the contract using rinkeby network flag (npx hardhat run scripts/deploy.js --network rinkeby)
- Try to send some ethers to second account

backend 

npm install --save-dev hardhat @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers ethers

npx hardhat
 