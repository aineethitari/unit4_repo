# Quiz 71
## Code
```.py
import random


def dec2hex(digit:int):
    if digit<16:
        if digit < 10:
            return str(digit)
        else:
            hex_dig = 'ABCDEF'
        return hex_dig[digit-10]
    return None

# or def2hex(digit:int):
    # return '0123456789ABCDEF'[digit]


def get_rand_hex():
    return dec2hex(random.randint(0,15))

def get_sixtect_hex():
    group = "".join([get_rand_hex() for _ in range(4)])
    # for _ in range(4):
    #     group += get_rand_hex()
    return group

def get_ip_v6_address():
    ip = ":".join([get_sixtect_hex() for _ in range(8)])
    # for m in range(8):
    #     ip += get_sixtect_hex() + ":"
    return ip

def ipv6machine(N):
    output = [get_ip_v6_address() for _ in range(N)]
    # for _ in range(N):
    #     output.append(get_ip_v6_address())
    return output

print(ipv6machine(N=4))
```

<img width="764" alt="quiz071" src="https://github.com/aineethitari/unit4_repo/assets/112055062/ea1002c6-bdb2-4895-9724-a903d3a8e5e7">

![quiz071](https://github.com/aineethitari/unit4_repo/assets/112055062/a38b36c6-258f-40a6-bc83-2db3cb1aa4e7)

