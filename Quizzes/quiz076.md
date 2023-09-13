# Quiz 76
![2022  Quizzes (26)](https://github.com/aineethitari/unit4_repo/assets/112055062/ec032445-271c-417d-88ee-cb2afd6cffbc)
## Code
```.py
def error_check(data:str):
    error = False
    copy_len = len(data)//3
    for i in range(copy_len):
        if data[i] != data[i+copy_len] or data[i] != data[i+(copy_len*2)]:
            error = True
    return error

data_1 = "100111001011001110010110011100101"
data_2 = "011101111101110111110111001111"
test1 = error_check(data_1)
print(test1)
test2 = error_check(data_2)
print(test2)
```
![quiz076](https://github.com/aineethitari/unit4_repo/assets/112055062/01d19e0a-af87-4bb8-9f61-854d155a34cc)

<img width="757" alt="quiz076" src="https://github.com/aineethitari/unit4_repo/assets/112055062/646c29bb-5c1f-4c77-b5e5-c8d5406508ff">
