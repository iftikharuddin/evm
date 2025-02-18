# Transactions

Think of a transaction like sending a special digital letter. Here's what happens:

1. When you want to send ETH or interact with a smart contract, you create a transaction. It's like filling out a form with:
   - Who it's from (your address)
   - Who it's to (recipient's address)
   - How much ETH you're sending
   - Your signature (to prove it's really from you)

2. Every transaction costs a small fee called "gas" - think of it like paying postage for a letter. The more complex your transaction (like interacting with smart contracts), the more gas you need to pay.

3. There are three main types of transactions you can make:
   - Simply sending ETH to someone else
   - Deploying a new smart contract
   - Interacting with an existing smart contract

4. Once you submit your transaction:
   - It gets broadcast to the network
   - Validators (like digital postal workers) pick it up and process it
   - When validated, your transaction gets added to a block and becomes permanent
   - The network updates everyone's balances accordingly

For example, if Bob wants to send 1 ETH to Alice:
- Bob's account gets charged 1 ETH plus a small gas fee
- Alice receives exactly 1 ETH
- The gas fee gets split between the network (most is "burned") and the validator

