## A. Conceptual Knowledge
1. What is a smart contract? How are they deployed? You should be able to describe how a smart contract is deployed and the necessary steps. 

- A smart contract is a concept in the blockchain system, a program that is executed autonomously according to rules set by code or other means in advance, without the intervention of a third party. The concept itself is not new; a simple example would be a vending machine. In recent years, however, the term "smart contract" generally refers to a self-executing program on a blockchain system according to rules set by code.
- Smart contracts are deployed by writing and recording code content on the blockchain. For example, first you write the code in solidity. Next, the code is compiled by EVM into EVM binary code. Finally, you complete the deployment by executing a transaction with the gas fee to record it in the chain.

2. What is gas? Why is gas optimization such a big focus when building smart contracts?

- The gas fee is the fee paid to the miner or validator when it executes a transaction and changes the state of the blockchain. The more transactions are executed, the higher the gas fee. The higher the gas fee offered, the stronger the incentive for the miner or validator to run the Node and execute that transaction.
- Since smart contract deployment transactions are more data intensive than simple money transfer transactions, the gas fee is also likely to be higher. Therefore, optimizing gas fees is very important.

3. What is a hash? Why do people use hashing to hide information?

- A hash is a unique string of fixed length that identifies data and is generated through a hash function that utilizes a hash algorithm such as sha256. There is a one-to-one correspondence between a piece of data and the hash generated from it. Using this property, blockchains, for example, ensure the invariability of blockchains by creating hashes from block numbers, nonce, data, and the hash of the previous block.
- Also, hash, unlike encryption, is irreversible. Therefore, the use of hash to hide information is very important because hashing allows verification of the correctness of data without disclosing the original data content.

4. How would you prove to a colorblind person that two different colored objects are actually of different colors?

- First, prepare two balls of different colors. (Assume that all factors other than color, such as size and shape, are the same.)
Next, I ask my colorblind partner to hold one ball in his/her right hand and the other in his/her left hand, and perform either "swap the balls" or "do not swap the balls" without being seen by me.
Then, I will answer whether he/she switched the ball or not.
By repeating this, I can prove that I can distinguish colors. 
Because if I could not distinguish the colors and had to guess, for example, the probability that I would get all the answers correct after 30 repetitions would be very small, 1 in 1073741824. 
But in fact I can say the correct answer 30 times and prove to my colorblind partner that I can tell the colors.

