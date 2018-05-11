# chain-data  

geth  --datadir "./chain" init init.json

geth --identity "scy" --rpc --rpccorsdomain "*" --datadir "chain" --port "30303" --rpcapi "db,eth,net,web3,personal,miner" --rpcport "8545" --networkid 95518 console 2>>geth.log

允许外网访问：geth --identity "scy" --rpc --rpccorsdomain "*" --datadir "chain" --port "30303" --rpcapi "db,eth,net,web3,personal,miner" --rpcport "8545" --rpcaddr "0.0.0.0" --networkid 95518 console 2>>geth.log 

tail -f geth.log 
