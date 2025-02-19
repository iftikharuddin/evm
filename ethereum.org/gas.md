# Gas and fees

Let's dig into Ethereum gas and fees in simple terms, along with important security considerations for auditors! 

1. **What is Gas? 🔑**
- Like fuel for a car, gas powers Ethereum operations
- Every transaction needs gas to run
- Paid in ETH, usually measured in "gwei" (1 billionth of ETH)

👮 **Security Note**: Check for gas-related attacks like:
- DoS through high gas consumption
- Gas griefing attacks
- Functions that could run out of gas unexpectedly

2. **Gas Fee Calculation 💰**
- Total Fee = (Base Fee + Priority Fee) × Gas Used
- Base Fee: Set by protocol, gets burned
- Priority Fee: Optional tip to validators

👮 **Security Note**: Look for:
- Gas exhaustion vulnerabilities
- Unbounded loops that could exceed block gas limits
- Functions that could become too expensive to call

3. **Base Fee Mechanism 📈**
- Changes based on network demand
- Can increase up to 12.5% per block
- Gets burned (removed from circulation)

👮 **Security Note**: Check for:
- Functions that might become unusable during high gas periods
- Logic that depends on specific gas costs
- Assumptions about base fee in contract logic

4. **Priority Fees (Tips) 🎯**
- Extra payment to validators
- Higher tips = faster processing
- Optional but recommended

👮 **Security Note**: Watch for:
- Front-running vulnerabilities
- MEV (Miner Extractable Value) exposure
- Transaction ordering dependencies

5. **Gas Limits ⚠️**
- Maximum gas allowed per transaction
- ETH transfer = 21,000 gas
- Complex contracts need more

👮 **Security Note**: Critical to check:
- Out-of-gas conditions in loops
- Array operations that could exceed limits
- Cross-contract calls that might fail

6. **Important for Security Researchers 🔍**
- Always test contracts under different gas conditions
- Check for gas-intensive operations that could be exploited
- Look for ways to optimize gas usage without compromising security
- Verify gas refund mechanisms
- Check for proper gas estimation in complex operations
- Look for potential DoS vectors through gas manipulation
- Verify handling of failed transactions
- Check for proper gas limit calculations in loops and recursive calls

Remember: Gas is a critical security component in Ethereum. Many vulnerabilities come from improper gas handling or assumptions about gas costs!
