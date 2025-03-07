# Connecting-to-Databases

### MySQL 

mysql-cli install :   
```sh
sudo dnf install mariadb105 -y
```
  
ElastiCache for Redis cli install :  
```sh
sudo yum install gcc jemalloc-devel openssl-devel tcl tcl-devel clang wget
wget https://github.com/valkey-io/valkey/archive/refs/tags/8.0.0.tar.gz
tar xvzf 8.0.0.tar.gz
cd valkey-8.0.0
make valkey-cli CC=clang BUILD_TLS=yes
sudo install -m 755 src/valkey-cli /usr/local/bin/
```

`If you install redis6 on Amazon Linux 2023, you can now use the command redis6-cli instead of valkey-cli:`
```sh
redis6-cli -h Primary or Configuration Endpoint --tls -p 6379
```
