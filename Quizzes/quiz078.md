# Quiz 78
## Code
```.py

def Layer4_firewall(data:str):
    dec = 0
    for i in range(0, 16):
        dec += int(data[i]) * (2 ** (15 - i))

    real_data = ""
    for i in range(0,len(data)-16):
        real_data += data[i+16]

    if dec == 80 or dec == 22123:
        error = "Allowed"
        msg = f"{real_data}"

    else:
        error = "Filtered"
        msg = "None"

    return error, msg


data = "100111001011001110010110011100101"
x = Layer4_firewall(data)
print(x)
```
<img width="754" alt="quiz078" src="https://github.com/aineethitari/unit4_repo/assets/112055062/eb27cc71-cab5-47fc-ad0e-77f649230946">

![quiz078](https://github.com/aineethitari/unit4_repo/assets/112055062/dea44351-0647-4b77-b6a6-bf04709e431e)
