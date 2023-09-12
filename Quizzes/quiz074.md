# Quiz 74
![2022  Quizzes (24)](https://github.com/aineethitari/unit4_repo/assets/112055062/905e0d2c-788c-4356-b4e2-5aef7632c328)
## Code
```.py
def build_data_pkg(mac_rx, ip_rx, mac_sx, ip_sx, data):
    output = []
    def msg(load_data,index):
        return f"{mac_rx}|{ip_rx} | {mac_sx} | {ip_sx} | {index} | {load_data}"

    for i in range(0,len(data), 4):
        load_data = data[i:i+4]
        index = i//4
        output.append(msg(load_data,index))

    return output

mac_rx = "AA:BB:CC:DD:EE:FF"
ip_rx = "10.0.0.1"
mac_sx = "11:22:33:44:55:66"
ip_sx = "10.0.0.2"
data = "This is a different test"

test = build_data_pkg(mac_rx, ip_rx, mac_sx, ip_sx, data)
print(test)
```
<img width="852" alt="quiz074" src="https://github.com/aineethitari/unit4_repo/assets/112055062/203920cb-77b3-416a-ad91-e3ea94a78f21">

