# Solving Boolean SAT Problem using Grover's Algorithm 

## Problem 

Frank wants to throw a dinner party to celebrate Alice and Bob’s engagement. He is also considering inviting their mutual friends Charles, Dave and Eve. However, he is aware that Charles will come to the party only if Dave comes without Eve. Frank wants to know what possible combinations of invitations he can write for his friends Alice, Bob, Charles, Dave and Eve.

Help Frank calculate all the possible combinations using Grover’s algorithm.

## Solution Roadmap 

- We first reformulate the problem into a boolean algebraic expression, this will make it simpler to construct an oracle. We also assign each person a qubit. 
- We then create an oracle based on the boolean expression. Luckily in our case we can create a phase oracle wothout the use of any ancilla and just the 5 qubits assigned to each person. 
- We the create the standard reflector used in Grover's Algorithm. 
- We create a sequential circuit of oracle and reflectors. The number of iterations are calculated using the complexity of the Grover's Algorithm and run the respective number of times. 
- We run the algorithm on the qasm simulator and obtain logically correct results with considerably decent accuracy. 
