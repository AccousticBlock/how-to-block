### how to make 2 connected peers in an instance


로컬노드1실행: 
./build/bin/geth --datadir ./tempdata/node1 init ../genesis.json 
./build/bin/geth --datadir ./tempdata/node1 --nodiscover console --port 30305

로컬노드2실행: 
./build/bin/geth --datadir ./tempdata/node2 init ../genesis.json
./build/bin/geth --datadir ./tempdata/node2  --nodiscover console --port 30306

로컬노드3실행: 
./build/bin/geth --datadir ./tempdata/node3 init ../genesis.json
./build/bin/geth --datadir ./tempdata/node3  --nodiscover console --port 30307

로컬노드2 console에서 admin.addPeer(‘로컬노드1주소’); // RLPx listener up 출력값

양쪽 노드 console에서 admin.peers 출력

*Genesis block 세팅
Geth실행시 init 값으로 geneis.json파일을 읽어 세팅하거나,
옵션값을 주지 않으면 core/geneis.go 파일 기반 세팅.

*마이닝
personal.newAccount()
miner.setEtherbase(‘account address’);
miner.start()
miner.stop()

Geth 트랜잭션 발생 예제
https://steemit.com/kr/@sangphilkim/geth
