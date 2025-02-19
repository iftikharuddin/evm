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

____
### Summary new version

📝 **Basic Transaction Types:**
1. Regular Transfer: Just sending ETH from you to someone else
2. Contract Deployment: Creating a new smart contract
3. Contract Interaction: Using an existing smart contract

🏷️ **What Every Transaction Includes:**
- From: Your address
- To: Recipient's address (or empty for contract deployment)
- Value: Amount of ETH to send
- Gas Limit: Maximum computing power you'll pay for
- Nonce: Your transaction counter (prevents replay)
- Signature: Your digital proof of authorization

⚡ **Transaction Evolution:**
- Type 0 (Old School): Basic transactions
- Type 1 (Upgraded): Added access lists for better gas efficiency
- Type 2 (Modern): Current standard with better fee handling
  - Splits fees into base fee + priority fee
  - More predictable costs
  - Better during busy network times

💡 **When Interacting with Contracts:**
- The data field tells the contract what to do
- First part (4 bytes): Which function to call
- Rest of data: The function's parameters (like amount, address)

Think of it like sending a smart letter that can either:
- Transfer money
- Create a new service
- Use an existing service
