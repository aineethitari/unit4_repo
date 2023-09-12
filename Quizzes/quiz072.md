# Quiz 72
![2022  Quizzes (22)](https://github.com/aineethitari/unit4_repo/assets/112055062/c2b23bef-c15b-4623-beca-cd8b8b82ba21)

## Code
```.py
import random

def macGenerator(N: int):
    mac_list = []
    hex_characters = '0123456789ABCDEF'

    for _ in range(N):
        mac = ""
        for _ in range(6):
            two_digit = ''.join(random.choice(hex_characters) for _ in range(2))
            mac += two_digit
            if _ < 5:
                mac += ":"
        mac_list.append(mac)

    return mac_list

mac_addresses = macGenerator(N=10)
for mac in mac_addresses:
    print(mac)
```

![quiz072](https://github.com/aineethitari/unit4_repo/assets/112055062/365bcc27-474c-4b12-ab68-65eab7330b35)

<img width="924" alt="quiz072" src="https://github.com/aineethitari/unit4_repo/assets/112055062/7de87960-1e2b-452e-8c3b-c307b700a46f">
