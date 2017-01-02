docker run  -t -i mysql /bin/bash
docker run --dns-opt=/etc/resolv.conf -t -i mysql /bin/bash
设置DNS服务器
docker run --dns=10.17.220.80 -t -i mysql /bin/bash

docker exec -it zabbix-server-mysql bash

