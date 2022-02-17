# 2022/2/16 stop generate block
```
Signed recently, must wait for others 
INFO [02-17|17:49:24.074] Sealing paused, waiting for transactions 
INFO [02-17|17:49:24.074] Signed recently, must wait for others 
以太坊私链昨天停止出块了，51个交易在pending里
原因是签字节点之前没有互通
163跟173居然不互通，把这两台机器上的签字节点迁移到172上，再重启94上的两个签字节点就好了
```
https://www.cnblogs.com/informatics/p/10417121.html

https://lessisbetter.site/2018/12/11/ethereum-design-of-txpool/
