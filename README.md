# Python Installing on linux

## Commands


__1. Updating repository:__</br> 
```sudo apt update```

__2. Installing python:__</br> ```sudo apt install python3```

__3. Checking python installed:__</br> ```python3 --version```

__4. PIP installation:__ </br> ```sudo apt install python3-pip```

__5. Venv interpreter package:__</br> ```sudo apt install python3.10-venv```

</br>

## Creating venv interpreter vs code:

__1. Go back to root folder of your program files:__ </br> ```You can use cd ..```

__2. Create interpreter:__ </br>```python3 -m venv my_venv_```

__3. Selecting my_venv:__ </br>```Hover on bottom status bar, left corner. You can look interpreter path. Click on it and click enter interpreter then select my_venv/bin/python3 ```


</br>

## python app

```
  print("============Get your GPA==============")

grades = {
    "A+": 4.00,
    "A": 3.75,
    "A-": 3.50,
    "B+": 3.25,
    "B": 3.00,
    "B-": 2.75,
    "C+": 2.50,
    "C": 2.25,
    "D": 2.00
}

print("Enter grades A+ to D\nIf you want to exit enter E\nTo enter another semester result enter y.")
def cgf():
    global GPA
    result = 0
    i = 0
    while i <= 2:
        x = input("Enter grades: ")
        if x == "E":
            break
        else:
            a = grades.get(x)
            result = result + a  
        i = i + 1
    GPA = result / i

# print()
cnt = 0
cg = 0
i = 1
while i != 2:
    cgf()
    i = int(input("1. To enter another block of grades\n2. Enter 2 to exit\nChoose your option: " ))
    if i == "1":
        cnt = cnt + 1
        cg = cg + GPA
        cgpa = cg / cnt
        continue
    elif i == 2:
        break
    else:
        print("Wrong input")
```


## Mongodb django tutorial
```
https://www.mongodb.com/compatibility/mongodb-and-django
```
