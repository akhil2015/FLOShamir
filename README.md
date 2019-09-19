# FLO-Shared-Secret
This app allows you to encrypt, store, and decode a secret on the FLO blockchain. 

In cryptographic terms, a "shared secret" is a secure piece of data known only to a trusted group of individuals. The secret can be a password, a passphrase, a large number, or a collection of randomly chosen bytes. The secret is encrypted by splitting it into a set number of keys ("n") that can distributed to a group of keyholders ("m"). The keyholders can then recombine the keys to decrypt the secret.

Built using Shamir's Secret Sharing algorithm, this app stores the encrypted secret message on the FLO blockchain and splits it into keys which can be distributed and recombined to decrypt the secret. The secret can be as large as 1040 bytes. Once stored to the FLO Blockchain, the secret cannot be altered and it is accessible from anywhere.

## Requirements
1. Linux operating system (working on a cross platform version).
2. You need to run a full flo-qt wallet to use the app. Download it from here https://github.com/floblockchain/flo
3. FLO cryptocurrenty to create the tranaction on the FLO Blockchain

**WARNING: Currently the app is using the testnet**

## Usage
1. Clone/download this repository. (https://github.com/akhil2015/FLO-shared-secret/)
2. Run the binary file. (FLO_Secret)

**To create the Shared-Secret**

1. click on POST to create a new Shared Secret message 
2. You will get a pdf containing your Secret ID and the shares of the keys used to encrypt it.
3. You should destroy the pdf once the shares have been distributed.

**To read the Shared Secret**

1. Click on GET to read the message.
2. Enter the Secret ID and shares of the keys
3. You should get a screen with the secret message displayed there.

## Source code
For Source code of the App is main.py
