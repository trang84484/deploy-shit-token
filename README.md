
# Deploy Shit Token

## Overview

**Deploy Shit Token** is a simple demo project for deploying a custom token on the Aptos blockchain. This project serves as a basic example for creating and deploying a token using Move smart contracts on Aptos.

## Features

-   Deploy a sample token on Aptos
    
-   Basic token functionality (mint, transfer, burn)
    
-   Uses Move programming language
    

## Requirements

Before running this project, ensure you have the following installed:

-   Aptos CLI
    
-   Move Language & Framework
    
-   Rust (for building and testing Move contracts)
    
-   An Aptos wallet (for deploying the token)
    

## Installation

1.  Clone this repository:
    
    ```
    git clone https://github.com/trang84484/deploy-shit-token.git
    cd deploy-shit-token
    ```
    
2.  Set up Aptos CLI and configure your account:
    
    ```
    aptos init
    ```
    
3.  Compile the smart contract:
    
    ```
    aptos move compile
    ```
    
4.  Deploy the token to the Aptos blockchain:
    
    ```
    aptos move publish --named-address deployer=your-account-address
    ```
    
5.  Mint tokens to your account:
    
    ```
    aptos move run --function-id 'deployer::shit_token::mint' --args address:your-account-address u64:1000
    ```
    
6.  Transfer tokens:
    
    ```
    aptos move run --function-id 'deployer::shit_token::transfer' --args address:recipient-account u64:amount
    ```
    

## Usage

-   Customize the `shit_token.move` file to modify token parameters
    
-   Run `aptos move test` to test the contract
    
-   Use Aptos Explorer to track transactions
    

## License

This project is licensed under the MIT License.
