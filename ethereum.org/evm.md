# Ethereum Virtual Machine (EVM)

Think of the EVM like a giant, shared computer that runs across the entire Ethereum network. Here's how it works:

1. **What it Does**
   - It's like a special computer program that runs on every Ethereum computer (node)
   - It makes sure smart contracts (programs on Ethereum) run exactly the same way everywhere
   - It's like a referee making sure everyone follows the same rules

2. **How it Works**
   - Instead of just tracking money like Bitcoin, it can run actual programs
   - It uses "gas" to measure how much computing power is needed
   - More complex operations cost more gas, which helps prevent overload

3. **State Changes**
   - Think of it like a massive spreadsheet that gets updated
   - When someone runs a transaction or smart contract:
     - The EVM reads the current state
     - Runs the instructions
     - Creates a new state with the changes

4. **Types of Actions**
   - You can send regular transactions (like sending ETH)
   - Or you can create and run smart contracts
   - Every action changes the "state" in a predictable way

The cool thing is that everyone running an Ethereum node will get exactly the same result when running the same code - it's like having thousands of computers all agreeing on what happened!

Think of the EVM like a special calculator that works in very specific ways:

1. **The Stack**
   - It's like a stack of cards where you can only work with the top cards
   - Each "card" holds a large number (256 bits)
   - You can stack up to 1024 items
   - Perfect for handling cryptographic operations

2. **Memory Types**
   - **Temporary Memory**: Like a scratch pad
     - Gets erased after each transaction
     - Used for temporary calculations
   
   - **Storage**: Like a permanent hard drive
     - Stays around forever
     - Each smart contract has its own storage
     - This is where important data is kept

3. **Basic Operations**
   - Can do simple math (ADD, SUBTRACT)
   - Can do logical operations (AND, OR, XOR)
   - Has special blockchain operations like:
     - Checking addresses
     - Looking up account balances
     - Getting block information

4. **Different Versions**
   - The EVM has been built in many programming languages
   - All versions must work exactly the same way

____

## OPCODES

Think of opcodes like the basic instructions that the Ethereum computer understands. Here are the main categories:

1. **Basic Math Operations**
   - ADD (01): Adds two numbers
   - MUL (02): Multiplies two numbers
   - SUB (03): Subtracts numbers
   - DIV (04): Divides numbers
   - These are like your calculator's basic functions!

2. **Stack Operations**
   - PUSH (60-7F): Puts a value onto the stack
   - POP (50): Removes a value from the stack
   - DUP (80-8F): Makes a copy of a value
   - SWAP (90-9F): Switches positions of values
   - Like organizing a stack of cards!

3. **Memory and Storage**
   - MLOAD (51): Reads from temporary memory
   - MSTORE (52): Writes to temporary memory
   - SLOAD (54): Reads from permanent storage
   - SSTORE (55): Writes to permanent storage
   - Like reading and writing to a computer's memory!

4. **Blockchain-Specific**
   - ADDRESS (30): Gets the current contract's address
   - BALANCE (31): Checks an account's balance
   - TIMESTAMP (42): Gets the current block time
   - BLOCKHASH (40): Gets a block's hash

5. **Control Flow**
   - JUMP (56): Moves to a different part of the code
   - RETURN (F3): Ends execution and returns data
   - STOP (00): Stops execution
   - Like traffic signals for the code!

Each instruction costs a certain amount of "gas" to run, which helps prevent infinite loops and ensures efficient code. It's like paying a small fee for each computer operation!