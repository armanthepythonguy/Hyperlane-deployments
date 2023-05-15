## Adding new warp-route pull request
Please, go through these steps before you submit a PR.
Check this link, if you have faced any difficulties :- 
https://docs.hyperlane.xyz/docs/deploy/deploy-warp-route/deploy-a-warp-route

With this PR, you are trying to add a new warp-route to the Hyperlane protocol. Other members can fetch your given details and can use it in their respective projects for interchain communication. Thus make sure your are suubmitting correct details.


Please make sure you are aligning with the below given points:- 
1. Make sure that your PR is not a duplicate.
2. Make sure that you have succesfully deployed warp-route onto Hyperlane.
3. Make sure you have deployed all the important contracts needed for Hyperlane deployment.
4. Make sure you have all the important contract addresses and info about the chain as you will be adding it the repo.
5. Have you tried testing your deployment by making some interchain interactions? If yes please upload some proofs.
6. Have you verified your smart contract on the network specific block explorers ? If not, please do it because the team can check and approve your PR faster.



Fillup these details before submitting the PR:-
1. Token Name :- <Your token name>
2. Chains :- <Chains used in this warp-route>
3. router contract address on  parent chain:- <Your router contract address on parent chain>
4. router contract address on remaote chain:- <Your router announce contract address on remote chain>



You need to make changes to the warp-routes.json file. With all the important details you need to add a registry to it:-
```
  
            {
                "name":"Demo",
                "chains":["parent chain", "remote chain"],
                "config":{
                  "parent-chain-name": {
                    "router": "router contract address on parent chain",
                    "tokenType": "collateral"
                  },
                  "remote-chain-name": {
                    "router": "router contract address on remote chain",
                    "tokenType": "synthetic"
                }
              }
          }
```
