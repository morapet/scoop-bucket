# scoop-bucket

for installation of scoop on windows please see [scoop](https://scoop.sh/)
 
#configure your git and copy your private key into id_rsa from github or your linux machine

* C:\Users\my\.ssh\id_rsa
* C:\Users\my\.gitconfig

# optional proxy 
* scoop config proxy webproxy.mycompany.com:8080
* $env:no_proxy = "mycompany.com"

# add repo
```
scoop bucket add synergy git@github.com:morapet/scoop-bucket.git
```
# run server
```
synergys --debug INFO --name server --address :8080-c configuration-demo.cfg --no-daemon
```
# run client
```
synergy-core.exe --client --name client <host>:8080
```
* host - server ip
