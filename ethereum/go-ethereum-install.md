# go and geth installation Instructions

### Ubuntu

go install
```
$ sudo add-apt-repository ppa:gophers/archive
$ sudo apt-get update
$ sudo apt-get install golang-1.9-go
$ export GOPATH=/usr/lib/go-1.9/
$ export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

geth install
```
$ sudo apt-get install -y software-properties-common
$ sudo add-apt-repository -y ppa:ethereum/ethereum
$ sudo apt-get update   
$ sudo apt-get install -y ethereum  
```
