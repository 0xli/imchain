# The blockchain to power Instant Messaging Application
An ethereum based side chain for messaging app

Run a private ethereum chain for developent, you are welcome to use it for your development or join us by running any kind of nodes:
1. bootnode
2. any full or light node for your own.
3. whisper node
4. swarm node

Check the status of imchain
http://gfax.f3322.org:3000

## 1. bootnode
you need a public ipv 4 address, any accessible ipv6 address works too
```
./bootnode --nodekey=boot.key -verbosity 5 -addr 10.0.0.232:30301
```
## 2. blockchain node of POA
run and join us (kad.network) for ethereum development
1. download geth:https://geth.ethereum.org/downloads/ 
2. download the genesys file devnet.json(https://github.com/allcomsh/imchain/blob/master/devnet.json)
3. initial directory,  
    geth --datadir node1 init devnet.json
4.  start geth   
Simplest way
```
../geth --datadir node1 --syncmode full --rpc --rpcapi "personal,ens,net,eth,web3"  --networkid 1515 --gasprice 1 --bootnodes "enode://eeddb5197f11b1c932b4613a937a9e2181e89a31a7526a661f146ce33414af4dfa5409639a24622559eb25f20fb16772ccdd81aa8d2764e2dbe77efa17d2295b@52.69.37.48:30301,enode://399c40c76434dbab54647d3310789e27bde00bb0ecff77c7d90efd76a862f99d6b2465c828d3eea59b7020329b765df7be480910e4e94fe0321e990aa6153eaa@118.190.79.30:30301" console
```
More options
``` 
 geth --datadir node1 --syncmode full --port 30303 --rpc --rpcaddr "0.0.0.0" --rpcport 8545 --rpcapi "personal,db,eth,net,web3,txpool,miner"  --networkid 1515 --gasprice 1  --lightserv 30 --rpccorsdomain "*" --bootnodes "enode://eeddb5197f11b1c932b4613a937a9e2181e89a31a7526a661f146ce33414af4dfa5409639a24622559eb25f20fb16772ccdd81aa8d2764e2dbe77efa17d2295b@52.69.37.48:30301,enode://399c40c76434dbab54647d3310789e27bde00bb0ecff77c7d90efd76a862f99d6b2465c828d3eea59b7020329b765df7be480910e4e94fe0321e990aa6153eaa@118.190.79.30:30301"console
```
> check peers
admin.peers.map(function(i){console.log(i.enode)})

## 3. whisper
### 3.1 web3.shh.subscribe need wss provider
- run geth with wss
  - --ws --wsport 8546 --wsapi shh,personal,ens,net,eth,web3,db,txpool --wsorigins * 
- nginx proxy for websocket
  - https://www.xncoding.com/2018/03/12/fullstack/nginx-websocket.html 
### 3.2 web3.shh 
-   https://web3js.readthedocs.io/en/v1.5.2/web3-shh.html#notification-returns
```
subscribe broadcast message
      FaxTokenImAPI.web3.shh.setProvider(new Web3.providers.WebsocketProvider('wss://geth.beagle.chat'));
      FaxTokenImAPI.web3.shh.subscribe('messages',{ symKeyID :symKeyID,topics:['0x12345678','0xffffffff']},callback);
subscribe to peer to peer message
      FaxTokenImAPI.web3.shh.setProvider(new Web3.providers.WebsocketProvider('wss://geth.beagle.chat'));
      FaxTokenImAPI.web3.shh.subscribe('messages',{ privateKeyID: shhKeyId},callback);

```
### 3. whisper references  
- https://github.com/allcomsh/Ethereum/blob/master/whisper.txt
- https://github.com/allcomsh/Ethereum/blob/master/whisper-mailserver.txt
## 4. swarm node
https://github.com/allcomsh/Ethereum/blob/master/swarm.txt
