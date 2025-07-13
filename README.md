# monad
This is my Git Repository.
Author - Rahul Sharma
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;


contract dynamicBytes{


    bytes public temp;

    constructor(){
        temp = "123abcd45";
    }

    function pushelement() public{
        temp.push("c");
    }

    function popElement() public{
        temp.pop();
    }

    function getlength() public view returns (uint){
        return temp.length;
    }

    function stopElement() public{
         temp.pop();
    }


  function getElement(uint _idx) public view returns(bytes1){
     return temp[_idx];
    }
    
}
