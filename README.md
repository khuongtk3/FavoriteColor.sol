# FavoriteColor.sol
Contract deployed via Web3 
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract FavoriteColor {
    mapping(address => string) public color;

    function setColor(string memory _color) public {
        color[msg.sender] = _color;
    }
}
