# CA6001I CA2 Assignment - Project 2

| <!-- -->    | <!-- -->    |
|-------------|-------------|
| Assignment      | CA6001I – CA2: Building a Hyperledger-based blockchain project         |
| Student         | Vipul Popat         |
| Student ID      | 21267549         |
| Email           | vipul.popat2@mail.dcu.ie         |


## Installation Pre-requisites
- Install hyperledger fabric on Windows 11 with WSL by following https://dev.to/hannudaniel/using-the-hyperledger-fabric-test-network-on-windows-11-with-wsl-2cac
- Clone the repository https://github.com/hyperledger/fabric-samples.git
- Clone the assignment repostory https://gitlab.computing.dcu.ie/popatv2/fabcar-extended.git
- Overwrite the file fabcar-extended\chaincode\fabcar.go to fabric-samples\chaincode\fabcar\go\fabcar.go
- Overwrite the file fabcar-extended\typescript-client to fabric-samples\fabcar\typescript\src\invoke.ts

## Running Hyperledger fabric
>$ cd fabric-samples\fabcar

>$ ./startFabric.sh

### This would start the hyperledger fabric using the approved docker imagees. Following would be available
- Succesfully running hyperledger fabric
- Smart Contract deployed

## Running the the typescript client
 >$ cd fabric-samples\fabcar\typescript

>$ npm run build

Enrolling an admin on the hyperledger network
>$ node dist\enrollAdmin

Registering an user on the hyperledger network
>$ node dist\registerUser

Invoke the smart contract to update the insurer
>$ node dist\invoke

Query all the car data on the blockchain
>$ node dist\query

## Stopping the hyperledger fabric
>$ cd fabric-samples\fabcar

>$ ./networkDown.sh




