# Instructions  

Create transactions spending to and from a Nested Segwit Multisig address on testnet.

Fill in the information about your transactions and copy any bitcoin-cli logs into the logs.txt file.

  ## Steps
  1. Write out your multisig script
  2. Encode your multisig script as a nested segwit (P2SH-P2WSH) bech32 address
  4. Lock coins to your P2SH-P2WSH address
  5. Unlock the coins from your P2SH-P2WSH address by spending them back to yourself (you can try using PSBT for this, it makes it easier in some ways but harder in others)

## Fill in the following questions about your Transactions and non-standard Script

1. Write out your multisig script with opcodes as it will be evaluated on the stack, scriptSig then scriptPubKey:

e.g. a P2PK looks like this: 

scriptPubKey = \<pubkey\> OP_CHECKSIG

scriptSig = \<signature\> 

How it's evaluated on the stack = \<signature\> \<pubkey\> OP_CHECKSIG

2. Multisig scriptPubKey (locking script) in Hex: 

3. Multisig scriptSig (unlocking script) in Hex:

4. Multisig scriptPubKey encoded as a P2SH-P2WSH bech32 testnet address:

(Hint: the hash of the hex_string != the hash of the bytes, make sure you're hashing at the byte level)

5. PARSED Raw Unsigned Transaction spending TO your P2SH-P2WSH address (like nifty does in class, Version: 02000000 etc.):

6. BLOB Raw Unsigned Transaction spending TO your P2SH-P2WSH address:

7. BLOB Raw SIGNED Transaction Spending TO your P2SH-P2WSH address:

8. TXID of transaction spending TO your P2SH-P2WSH on testnet: 

9. PARSED Raw Unsigned Transaction spending FROM your P2SH-P2WSH address (like nifty does in class, Version: 02000000 etc.):

10. BLOB Raw Unsigned Transaction spending FROM your P2SH-P2WSH address:

11. PARSED Raw SIGNED Transaction spending FROM your P2SH-P2WSH address:

12. TXID of transaction spending FROM your P2SH-P2WSH on testnet:



