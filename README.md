# Security tools: Slither and Echinda
Slither is a security tool provided by Trail of Bits that does static analysis of smart contracts.
It examines the source code before the program runs using the the solidity compiler. This tool
detects vulnerabilities, suggests how to optimize your code, helping you to develop
better smart contracts. To learn more about Slither, visit
`https://github.com/crytic/slither`


## Technology Stack & Dependencies

- Solidity (Writing Smart Contract)
- [NodeJS](https://nodejs.org/en/) To create hardhat project and install dependencies using npm


### 1. Clone/Download the Repository

### 2. Install Dependencies:
```
npm install
```

### 3. Install Slither
- Install the solc compiler first then slither
```
brew tap ethereum/ethereum
```
```
brew install solidity
```
```
git clone https://github.com/crytic/slither.git
```
```
sudo python3 setup.py install
```
```
slither .
```
### Note:

Ensure you're in the correct directory, in this case the project folder. When running
`slither .` in your terminal, you may also run it as `slither your-contract.sol`
however it may run into issues with smart contracts that import other contracts. For
simplicity, it is recommended to run `slither .`

Once Slither has been properly ran in your terminal, a large amount of text in red, yellow,
and green will display potential vulnerabilities, pitfalls, warnings, and suggestions. Though this
is a very handy tool for smart contract security, it is not perfect. By no means is it
a catch-all solution to the security of your contracts. It is good practice to exhaust
all resources before pushing the final product to the main net.

### 4. Install and use Echinda 
- Install the solc compiler first then slither
```
docker pull trailofbits/eth-security-toolbox
```
```
docker run -it trailofbits/eth-security-toolbox
```
