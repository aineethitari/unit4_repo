# Quiz 73
![2022  Quizzes (23)](https://github.com/aineethitari/unit4_repo/assets/112055062/2e6786ac-1f35-47d5-a5e8-0fe3ae720c78)

## Code
```.py
from quiz070 import IPv4machine
def check_mac(mac:str)->bool:
    return len(mac)==17 and mac.count(":")==5
routing_table = {}
def get_ip(mac:str)->str:
    ip_out = 'Error'
    if check_mac(mac):
        if mac in routing_table.keys():
            ip_out = routing_table[mac]
        else:
            while True:
                ip = IPv4machine(N=1)
                if not ip in routing_table.values():
                    routing_table[mac] = ip
                    ip_out = ip
                    break
            return ip_out
```

<img width="1371" alt="quiz073" src="https://github.com/aineethitari/unit4_repo/assets/112055062/eb0f18e5-9932-4b28-b344-ba575bc357b9">
![quiz073](https://github.com/aineethitari/unit4_repo/assets/112055062/ae93a97f-60b6-45b1-a2ad-9887d347d231)
