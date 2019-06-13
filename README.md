# run and join us for ethereum development
1. download geth:https://geth.ethereum.org/downloads/ 
2. download the genesys file devnet.json and static-nodes.json here
3. initial directory,  
    geth --datadir node1 init devnet.json
4.    
 geth --datadir node1 --syncmode full --port 30303 --rpc --rpcaddr "0.0.0.0" --rpcport 8545 --rpcapi "personal,db,eth,net,web3,txpool,miner" --bootnodes "enode://11e1d914c7d4b09f5cbf6ff238ee9fede90fc8cb60484856848421971203b58484023b44771161dc229447b398fbaf4b122611d282bda54555c3089cb3c294b6@118.190.79.30:30307" --networkid 1515 --gasprice 1  --lightserv 30 --rpccorsdomain "*" console

# imchain
a ethereum based side chain for messaging app

Run a private ethereum chain for developent, you are welcome to use it for your development or join us by running any kind of nodes:
1. bootnode
2. whisper node
3. swarm node
4. any full or light node for your own.

Check the status of imchain
http://gfax.f3322.org:3000

admin.peers.map(function(i){console.log(i.enode)})
