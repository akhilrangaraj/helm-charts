see https://github.com/revoltchat/self-hosted/


vortex
```
#!/bin/bash

docker run -d  --name vortex  -e WS_URL="wss://<host>" -e MANAGE_TOKEN="<token>" -e RTC_IPS="0.0.0.0,<external_ip>"  -p 8080:8080 -e RTC_MIN_PORT=10001 -e RTC_MAX_PORT=10100 -p 10001-10100:10001-10100/tcp -p 10001-10100:10001-10100/udp revoltchat/vortex:0.3.0-alpha.1
```
doesnt really work