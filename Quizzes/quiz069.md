# Quiz 69
![2022  Quizzes (19)](https://github.com/aineethitari/unit4_repo/assets/112055062/687cf287-58db-4f80-b9bc-bc872416d335)
## Code 
![IMG_7907](https://github.com/aineethitari/unit4_repo/assets/112055062/32ba2a93-52ad-4925-9760-65ba89f84c88)

```.py
index = 0
sales = input()
sales = sales.split(',')

small = float(sales[0])
big = float(sales[0])

for i in range(len(sales)):
    if float(sales[i]) < small:
        small = float(sales[i])
    if float(sales[i]) > big:![Uploading IMG_7907.JPG…]()

        big = float(sales[i])

diff = int(big-small)
print(diff)
```

<img width="529" alt="quiz069" src="https://github.com/aineethitari/unit4_repo/assets/112055062/c5d18c6f-de72-4514-85fb-61eff679c908">
