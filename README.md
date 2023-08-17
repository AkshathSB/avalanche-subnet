# Deploying a contract on a AVAL Subnet

To deploy a contract on the avalanche EVM subnet 

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has several functions for the DEFI game mainly having one function called the gains funciton where the players health can be increased to a max of 200 by gaining some "roidenergy".  This program helps me to understand the basic coding elements of Solidity such has creating user-defined functions and understanding the language and also learn how contracts are being transacted on the avalanche EVM subnet. 

## Getting Started

### Executing program

#### Creating a subnet
To create a subnet run:
``` shell
avalanche subnet create <subnet_name>
```
then a prompt is shown to enter a ChainId of your own choice
``` shell
you can type any sequential number of your choice for your ChainId
```
and then once your ChainId is created it prompts to create a token symbol of your choice
``` shell
Enter your token symbol
```
after your token symbol is created make sure to choose these options which will be prompted:
```shell
Use the latest version
Low disk use
Airdrop 1 million tokens to the default address (do not use in production)
no
```
Then your subnet is succesfully created subnet config

#### Deployin the subnet
To deploy the subnet run:
``` shell
avalanche subnet deploy <subnet_name>
```
once that is ran, it deploys the subnet to local network VMs
and then which are provided further details about the subnet such RPC URL, Chain ID, Network name etc, all which are 
helpful for linking the subnet network to your metamask.

#### Connecting the network to your metamask
To connect the subnet create a new network under networks and enter the requested details to which are all given back in your command prompt as mentioned above.

#### Compiling and deploying the contract over the subnet

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g.,Game.sol). 

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.17" (or another compatible version), and then click on the "Compile Game.sol" button.

Once the code is compiled, we need to change the environment to injected provider which opens the metmask asking for conformation to connect to the subnet once approved select the account with 1million tokens and the deploy the contract.

Once the contract is deployed, you can interact with it by calling the "gains" and other functions. Where the "gains" function helps the player to get more health using the "roid energy" which is limited using the require error handler. There are also other functions such as mint and burn fucntions to add or burn tokens to a requested account by providing the address respectively

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Akshath.SB  

@akshathbhandiwad2@gmail.com

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
