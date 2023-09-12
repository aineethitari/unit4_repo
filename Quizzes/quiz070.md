# Quiz 70
![2022  Quizzes (20)](https://github.com/aineethitari/unit4_repo/assets/112055062/1ce49799-9c2d-421f-9906-ee86cb5a01c9)
## Code
![IMG_7909](https://github.com/aineethitari/unit4_repo/assets/112055062/cb0e9149-8e67-452a-8f73-63d8f38b0a0a)
```.py
def IPv4machine():
    ips = []
    for a in range(256):
        for b in range(256):
            for c in range(256):
                for d in range(256):
                    ips.append(f"{a}.{b}.{c}.{d}")
    return ips

ip_addresses = IPv4machine()
print(ip_addresses)
```
<img width="1111" alt="quiz070" src="https://github.com/aineethitari/unit4_repo/assets/112055062/daef1c46-b7b9-439c-8aa6-74929b209fed">
