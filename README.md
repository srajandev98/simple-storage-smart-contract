# Simple Storage Smart Contract

The first line tells us that the source code is licensed under the MIT. Machine-readable license specifiers are important in a setting where publishing the source code is the default.

The next line specifies that the source code is written for Solidity version 0.4.16, or a newer version of the language up to, but not including version 0.9.0. This is to ensure that the contract is not compilable with a new (breaking) compiler version, where it could behave differently. Pragmas are common instructions for compilers about how to treat the source code (e.g. pragma once).

## What is a Smart Contract?
A contract in the sense of Solidity is a collection of code (its functions) and data (its state) that resides at a specific address on the Ethereum blockchain. 

## How does the above Smart Contract Work?
The line uint storedData; declares a state variable called storedData of type uint (unsigned integer of 256 bits). You can think of it as a single slot in a database that you can query and alter by calling functions of the code that manages the database. In this example, the contract defines the functions set and get that can be used to modify or retrieve the value of the variable.

To access a member (like a state variable) of the current contract, you do not typically add the this. prefix, you just access it directly via its name. Unlike in some other languages, omitting it is not just a matter of style, it results in a completely different way to access the member.
