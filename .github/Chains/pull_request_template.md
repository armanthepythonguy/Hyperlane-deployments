## Adding new chain pull request
Please, go through these steps before you submit a PR.
Check this link, if you have faced any difficulties :- 
https://docs.hyperlane.xyz/docs/deploy/deploy-hyperlane

With this PR, you are trying to add a new network to the Hyperlane protocol. Other members can fetch your given details and can use it in their respective projects for interchain communication. Thus make sure your are suubmitting correct details.


Please make sure you are aligning with the below given points:- 
1. Make sure that your PR is not a duplicate.
2. Make sure that you have succesfully deployed Hyperlane onto the new chain.
3. Make sure you have deployed all the important contracts needed for Hyperlane deployment.
4. Make sure you have all the important contract addresses and info about the chain as you will be adding it the repo.
5. Have you tried testing your deployment by making some interchain interactions? If yes please upload some proofs.
6. Have you verified your smart contract on the network specific block explorers ? If not, please do it because the team can check and approve your PR faster.



Fillup these details before submitting the PR:-
1. Chain Name :- <Your chain name>
2. Chain ID :- <Your chain ID>
3. RPC URL :- <rpc url of the network>
4. MailBox contract address :- <Your mailbox contract address on deployed chain>
5. ValidatorAnnounce contract address :- <Your validator announce contract address on deployed chain>
6. InterchainGasPayMaster contract address :- <Your InterchaingasPayMaster contract address on deployed chain>



You need to make changes to the chains.json file. With all the important details you need to add a registry to it:-
```
  
            {     
                "name":" Your chain name",
                "chainId": your chain id,
                "rpcUrls":[
                    "rpc url of your chain"
                ],
                "mailbox": "mailbox contract address on your network",
                "validatorAnnounce": "validatorannounce contract address on your network",
                "interchainGasPaymaster": "interchaingaspaymaster contract address on your network"
            }
```
