# Quiz 75
![2022  Quizzes (25)](https://github.com/aineethitari/unit4_repo/assets/112055062/e4394291-a302-4880-a8b5-c7bafe4f1475)
## Code
```.py
def tobinary(data: str):
    final = ""
    for i in range(len(data)):
        binary = ""
        ascii = ord(data[i])
        while ascii > 0:
            binary = str(ascii % 2) + binary
            ascii = ascii // 2
        if len(binary) != 8:
            binary = "0" * (8 - len(binary)) + binary
        final += f"{binary} "
    return final.rstrip() 

data = "Hello World!"
binary_out = tobinary(data)
print(binary_out)
```
<img width="939" alt="quiz075" src="https://github.com/aineethitari/unit4_repo/assets/112055062/b19c109b-325a-4c5a-82f9-aadc6f3f04e8">
![Uploading quiz075.JPG…]()
