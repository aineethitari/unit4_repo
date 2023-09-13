# Quiz 77

![2022  Quizzes (27)](https://github.com/aineethitari/unit4_repo/assets/112055062/c372864f-737f-4b6a-aa18-748cafd90f86)
## Code
```.py
def parity_check(data: str):
    count = 0
    error = True
    for i in range(len(data) - 1):
        if data[i + 1] == '1':
            count += 1

    if data[0] == '1':
        if count % 2 == 0:
            error = False
    if data[0] == '0':
        if count % 2 != 0:
            error = False

    return error

data_1 = "100111001011001110010110011100101"
data_2 = "011101111101110111110111001111"
x1 = parity_check(data_1)
x2 = parity_check(data_2)
print(x1)
print(x2)
```
![quiz077](https://github.com/aineethitari/unit4_repo/assets/112055062/d8db3d05-f1ab-4e65-b805-f0b7c1c1e054)
![quiz077](https://github.com/aineethitari/unit4_repo/assets/112055062/c64dbc51-96f7-471b-bfc7-7e26c19102ec)
