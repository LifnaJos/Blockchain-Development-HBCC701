# Experiment  No - 2 : Create a Blockchain using Python
* Date of Preparation : 1st week of August
* Date of Submission : 2nd week of August 
* Lab Objectives: To realize the basic techniques to build intelligent systems
* Lab Outcomes (LO): Demonstrate the concept of Blockchain in real-world Applications (LO4)

## Task to be performed : 
#### Step - 1 : Construct Merkle Tree 
1. Make a copy of this [Google Colab Notebook](https://colab.research.google.com/drive/1RDlF1gtFp7Bxlkn0IQv01muSbfuTSajh?usp=sharing)
2. Try to solve the errors in each of the 4 Programs
3. In the 4th Program - Constructing a Merkle Tree Root Hash, modify the code as follows:
  - Update the transactions list with valid entries. 
    - eg : transactions = ['A -> B : $10', 'B -> C : $5,'C -> A : $2']
  - Sample Transactions to be considered 
    -  T1 : Alice → Bob : $200;
    -  T2 : Bob → Dave : $500;
    -  T3 : Dave → Eve : $100
    -  T4 : Eve → Alice : $300;
    -  T5 : Roo → Bob : $50
  - Hash the transactions before combining them in the for loop
  - Print all the intermediate hash during the construction of the Merkle Tree Root Hash

#### Step - 2 : Run a Blockchain with one node 
1. Make a copy of this [Google Colab Notebook](https://colab.research.google.com/drive/17YNc9k4TBYqyuFb823w5lkEJu9bg8g5g?usp=sharing)
2. Try to solve the errors in given Program
3. After successful execution of the Program in Colab Notebook.
  - Add a method, create_Transactions
  - Mine the block only when the transaction list is not null.
  - Remove the transactions from the list of transactions before mining.
  - Modify the method, proof_of_work() to search for the golden nonce
  - Cryptographic Puzzle is to have “000” leading zeros in the Block Hash
4. Download the code - [blockchain.py](https://drive.google.com/file/d/1K3iVvJMmORB5ELfBrQESXbRLCCRIK7Id/view?usp=drive_link)
5. Update the code to incorporate the changes in step 3 to the code in step 4.
6. Follow the steps in [Manual](https://drive.google.com/file/d/1dNPlk0Bmel0ztwcHYyqEr8073VQUD6_A/view?usp=sharing) to demonstrate the working of Blockchain using Flask and Postman.

#### Step - 3 : Run a Blockchain with 3 peer nodes
1. Download the code from folder, [Lab_2_Step_2](https://drive.google.com/drive/folders/1htqRnrCS5PVbKnVT6cF8FrRAKRx3V2fW?usp=sharing)
2. Install requests in the virtual environment created in Step 1. ([Follow the instructions](https://drive.google.com/file/d/1dNPlk0Bmel0ztwcHYyqEr8073VQUD6_A/view?usp=sharing))
3. Run the files - hadcoin_node_5001.py, hadcoin_node_5002.py, hadcoin_node_5003.py in 3 different terminals.
4. Open Postman, from each node - invoke connect_node() and pass the peers as POST requests.
5. Perform the following functions
  - Add Transactions - invoke add_transactions() as a POST request.
  - mining - mine_block(),
  - fetch the chain - get_chain(),
  - replace the longest chain - replace_chain()
6. Modify the code such that transactions are removed after they are added to the block.

### Tools & Libraries used : 
* Install [Flask](https://flask.palletsprojects.com/en/2.1.x/quickstart/#about-responses) : pip install Flask
* Download [Postman](https://www.postman.com/)
* Python Libraries : datetime, jsonify, hashlib, uuid4, urlparse, request
* Install requests : pip install requests==2.18.4

### Instructions : 
Write theory for the following topics
1. Cryptographic Hash functions in Blockchain
2. [What is a Merkle Tree? How does a Merkle Tree work?](https://drive.google.com/file/d/1MERIb_UIOOXzvQ4VhdDirnv418JlJ68S/view?usp=sharing)
3. What is a Cryptographic Puzzle and explain the Golden Nonce
4. Benefits and Use cases of Merkle Tree
5. [What is a Blockchain? Explain the process of Mining](https://drive.google.com/file/d/1StlkB-IbXtnlUWQnR5CZ5VhDLwFADqZl/view?usp=sharing)
6. How to check the validity of blocks in a Blockchain
7. Challenges in P2P networks
8. How transactions are performed on the network?
9. Explain the role of mempools
10. Write briefly about the libraries and the tools used during implementation.

### Outcome :  
1. Understood the challenges in P2P networks, how transactions are performed and how a miner mines a block to be added in a blockchain.
2. Implemented a Cryptocurrency in Python using Flask, Postman and Python libraries such as datetime, jsonify, hashlib, uuid4, urlparse, request.
3. Successfully mined the blocks among a P2P network with 3 nodes.
4. Performed transactions via the network.
5. Successfully updated the block across the network
6. Attach the Theory, Program, and Output
(As per the instructions, submit a hard copy of the same).
