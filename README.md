Adding web3.js
First you need to get web3.js into your project. This can be done using the following methods:

npm: npm install web3
yarn: yarn add web3
pure js: link the dist/web3.min.js
After that you need to create a web3 instance and set a provider.

Most Ethereum-supported browsers like MetaMask have an EIP-1193 compliant provider available at window.ethereum.

For web3.js, check Web3.givenProvider.

If this property is null you should connect to a remote/local node.

// In Node.js use: const Web3 = require('web3');

let web3 = new Web3(Web3.givenProvider || "ws://localhost:8545");
That’s it! now you can use the web3 object.