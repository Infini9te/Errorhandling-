# Errorhandling
## Usage of Errors and Functions
This simple Solidity program demonstrates how errors are handled in the Solidity programming language. It shows the basic syntax and functionality of error handling, with a specific focus on using the require, revert, and assert keywords. The program aims to provide a practical example of how to handle errors effectively using these keywords.

## Description
This program is a simple contract written in Solidity, a programming language specifically used for creating smart contracts on the Ethereum blockchain. The contract includes three functions that demonstrate how to use three important keywords: require, revert, and assert. By studying this program, beginners can easily grasp the basics of Solidity programming. It serves as a starting point for them to build a strong foundation and eventually take on more complex projects in the future.

##Getting Started
###Executing Program
To run this program, you can use gitpod , an online Solidity IDE. To get started, go to https://jeffryanpol-soliditysta-sbt87u3aw59.ws-us98.gitpod.io/
After this, create a new file named errorhandling and follow this code: 

/ SPDX-License-Identifier: MIT
pragma solidity ^0.8.1;

contract ErrorHandlingExample {
    uint256 public count;

    constructor() {
        count = 0;
    }

    function modifyCount(uint256 newValue) external {
        count = newValue;
    }

    function testRequire(uint256 _value) public pure {
        require(_value > 5, "Input must be greater than 5");
    }

    function testRevert(uint256 _value) public pure {
        if (_value <= 5) {
            revert("Input must be greater than 5");
        }
    }

    function testAssert() public view {
        assert(count == 10);
    }
}

## Authors
SHUBHAM 

## LICENSE
This project is licensed under the MIT License - see the LICENSE.md file for details




