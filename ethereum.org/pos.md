# Proof of stake

Think of PoS like this:

1. Basic Concept
- Instead of using computer power (like old PoW system), validators must deposit 32 ETH as collateral
- It's like putting down a security deposit to become a trusted validator
- If validators do their job honestly, they earn rewards
- If they cheat, they lose their deposit!

2. How It Works
- Time is divided into 12-second slots and epochs (32 slots)
- For each slot:
  - One random validator is chosen to propose a new block
  - Other validators check if the block is valid
  - They vote (attest) whether they agree with the block
  - If enough validators agree, the block is added to the chain

3. Key Benefits
- More energy efficient (no heavy computing needed)
- More secure (cheating is very expensive)
- More decentralized (can run on a regular laptop)
- Less new ETH needs to be created
- Anyone with 32 ETH can participate (or join staking pools with less)

4. Security Features
- To attack the network, you'd need 51% of all staked ETH
- Bad behavior gets punished by:
  - Losing some or all staked ETH
  - Getting kicked out of the network
  - The more validators misbehave together, the bigger the punishment

5. Finality
- A transaction is "final" when it can't be changed
- Happens when 2/3 of validators agree on checkpoints
- Takes about 6.4 minutes under normal conditions

