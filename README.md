# mev-quiz

Test your knowledge, with the pure Novice version.  A Solidity dev could complete this in less than 10 minutes, as this is nothing more than structured motivation to read the Flashbots FAQ.

With more interest, may expand this to include Intermediate to Advanced tests.  Please submit a PR if you'd like to add to it

Resources:

- https://docs.flashbots.net/

## Novice Quiz

1. What software does a searcher run, to earn MEV from flashbots?
2. As a searcher, which testnet can I use for flashbots?
3. As a searcher, what is the name of the javascript library that I can use to send bundles?
4. As a searcher, what is the name of the python library that I can use to send bundles?
5. For a given MEV-mined block, what position is the bundle placed?
6. If I wanted to have the fastest connection to Flashbots relay, which geographic location should I place my servers?
7. Give an example transaction of a recent flashbots transaction mined after block 12,800,000 (not from FAQ, go see Etherscan)
8. What software does a miner run, to earn MEV from flashbots?
9. Starting from which block number can I backtest bundle strategies?
10. What URL do I use to send a GET request to access the most recent mined flashbot blocks?
	- Download Postman, https://www.postman.com/downloads/ copy paste me one of the most recent flashbot blocks in the above GET url.  It should look like this:
	```
	        {
            "block_number": 12809499,
            "miner_reward": "13897142429335872",
            "miner": "0xEA674fdDe714fd979de3EdF0F56AA9716B898ec8",
            "coinbase_transfers": "0",
            "gas_used": 100576,
            "gas_price": "138175533222",
            "transactions": [
                {
                    "transaction_hash": "0xa09823b9eb5e65f67ef4031e96bba55750e0448a343b5d56601fb803b10c1b42",
                    "tx_index": 0,
                    "bundle_type": "flashbots",
                    "bundle_index": 0,
                    "block_number": 12809499,
                    "eoa_address": "0x2d0862Ef64149EEbBb1222BbB556f50e81D1ba20",
                    "to_address": "0x4d246bE90C2f36730bb853aD41d0a189061192d3",
                    "gas_used": 100576,
                    "gas_price": "138175533222",
                    "coinbase_transfer": "0",
                    "total_miner_reward": "13897142429335872"
                }
            ]
        },
	```
11. If I wanted to backrun an oracle, what do I put inside the "signBundle" function?  Describe it in words, don't need the code.
12. How do I avoid losing sending tip money if the miner uses a contract as their coinbase?
13. What is the Flashbots discord URL?  Copy paste the latest alert from the bundle-alerts channel
14. What is the URL for data metrics for flashbots?  What is the last 30 days extract MEV?
15. What is the URL for flashbots dashboard?  How many unique searchers are there in the relay at this moment?
16. What is the URL for the flashbots bundle explorer?  Screenshot a bundle inspection
17. What is the URL for the flashbots github?  Which code is an example demo of arbitrage?
18. Create a python script to interact with flashbots testnet relay
19. Create a javascript script to interact with flashbots testnet relay

Bonus Questions:

20. How do I avoid getting salmonella'd / lose ETH, in a bundle?
21. How do I avoid getting my uncled transactions sniped/stolen?
