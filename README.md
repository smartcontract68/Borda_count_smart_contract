# Borda_count_smart_contract


How can I use this library and go?
=====================================

You need to run 'Geth' in the background:

1. geth <OPTIONAL: --dev/testnet> --rpc --rpcapi="db,eth,net,web3,personal" --rpcport "8545" --rpcaddr "127.0.0.1" --rpccorsdomain "*" console

Example: ./geth --dev --rpc --ipcpath "~/Library/Ethereum/geth.ipc" --rpcapi="db,eth,net,web3,personal" --rpcport "8545" --rpcaddr "127.0.0.1" --rpccorsdomain "*" console
 
2. Compile the .SOL, and send it to the Ethereum Network.

3. Update voter.html, administrator.html and live.html with the correct abi/contract address.

4. Voters open voter.html, and the Election Admin opens administrator.html

5. Each voter requires a votermod.txt document that contains random variables,
secret keys, public keys.


6. Voters can register and cast their vote.

An example 'votermod.txt' has been included, and a Java Program 'main.java' is included that can compute these numbers for the voter.


Complete election simulation for 5 condidates is included in the folder borda_count_5_candidates. The test code for 2, 3 and 4 candidates is included in other folders.
