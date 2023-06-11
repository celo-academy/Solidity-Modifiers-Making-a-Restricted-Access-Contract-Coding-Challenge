## Introduction

Solidity is the primary language used for creating smart contracts on blockchain platforms like Celo. One of the key features of Solidity is the use of modifiers to add prerequisites to function calls. In this challenge, you will build a contract that leverages modifiers for restricted access control.

## Problem Statement

Develop a contract that simulates a simple voting system with the following requirements:

1. The contract should allow the owner to add candidates for voting.
2. Voters should be able to vote for these candidates.
3. The contract should prevent non-owners from adding candidates.
4. The contract should prevent voters from voting more than once.
5. The contract should contain a function to get the total votes a candidate has received.
6. The contract should have a function to declare the winner based on the highest votes.

## Hints

- Use `modifier` keyword in Solidity to define your access control modifier for the contract owner.
- You can use the `msg.sender` global variable to verify the sender's address.
- Keep track of voters and their voting status using a `mapping`.
- Use a `struct` to represent a candidate with properties such as id and vote count.
- Keep a list of candidates in an array for easy management.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and meet all the requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Please note, this challenge focuses on modifier usage and doesn't cover important aspects like security, gas optimization, and contract upgradability, which are critical for real-world contract deployment on the Celo platform.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your voting system contract. Also, include any notes or comments you think are necessary for understanding your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.
