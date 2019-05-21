mkdir node1
copy static-nodes.json node1
geth --datadir node1 init devnet.json
geth --datadir node1 account new
修改 node1.bat，用上面命令返回的address替代unlock后面的账号 