#This is a basic application to test blockchain using Solidity programming language and an ethereum based lifecycle.

##Steps to install dev enviromnent:
1. ``` npm i -g ethereumjs-testrpc ```
2. ``` npm i -g truffle ```

##Steps to download and install dependencies of this project:
1. clone this repository using git: ``` git clone https://github.com/alecventura/foodSafeEthereum.git foodSafe ```
2. install dependencies with node: ``` npm install ```

##Steps to run a simple test:

### Go inside the project folder on command line and type the commands:
#### Run the RPC server to simulate a blockchain with miners (do this one a separated terminal):
1. ``` testrpc ```

#### Now run the compile + deploy commands:
2. ``` truffle compile ```

3. ``` truffle migrate ```

#### Now you can access a javascript console just to make sure everthing is working:
4. ``` truffle console ```
1.1. ```javascript var fs; ```
1.2. ```javascript FoodSafe.deployed().then(function(deployed){fs=deployed;}); ```
1.3. ```javascript fs.AddNewLocation(1000, "The Producer", "Not very secret scret..."); ```
1.4. ```javascript fs.AddNewLocation(2000, "The Supplier", "Still not very secret scret..."); ```
1.5. ```javascript fs.AddNewLocation(3000, "The Store", "Even still not very secret scret..."); ```
1.6. ```javascript fs.GetLocation.call(0).then(function(retval){console.log(retval);}); ```
1.8. ```javascript fs.GetLocation.call(1).then(function(retval){console.log(retval);}); ```
1.9. ```javascript fs.GetLocation.call(2).then(function(retval){console.log(retval);}); ```

