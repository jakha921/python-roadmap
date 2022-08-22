# Python 3

## В этом модель мы разберем

### Содержание курса

- [___Ввод и вывод данных___](#Ввод-и-вывод-данных)
- [___Переменный___](#Переменный)
- [___Типы данных (int, float, str, bool)___](#Типы данных)
    - [___Тип integer & float___](#Integer-&-float)
    - [___Тип string___](#String)
    - [___Тип boolean & операторы сравнение___](#Boolean-&-операторы-сравнение)
- ___Условный оператор___
- ___Цикл for и while___
- ___Строковый тип данных (str)___
- ___Списки___
- ___Функции___
- ___Работа над проектом___

---

## Ввод и вывод данных

    # print
    from statr to end 
    print("Hello, world") / print('Hello, world')
    print("hi", args)

    # input
    print("Whats your name?")
    name = input()  / input("Whats your name?)
    print("My name is", name)

    # set, end, \

HW

    Распечатать Елку из *
      
    # Выести так же и наоборот
    I
    Love
    Python

    Hi, Jakhongir

    math, \text, a+b=c, 
  
    print('a', 'b', 'c', sep='*') / end='#'
    print('d', 'e', 'f', sep='**') / end='##'

    print('Mercury', 'Venus', sep='*', end='!')
    print('Mars', 'Jupiter', sep='**', end='?')

    print('a', 'b', 'c', sep='*')
    print('d', 'e', 'f', sep='**', end='')
    print('g', 'h', 'i', sep='+', end='%')
    print('j', 'k', 'l', sep='-', end='\n')
    print('m', 'n', 'o', sep='/', end='!')
    print('p', 'q', 'r', sep='1', end='%')
    print('s', 't', 'u', sep='&', end='\n')
    print('v', 'w', 'x', sep='%')
    print('y', 'z', sep='/', end='!')
    
    language = 'Python'
    language = 'Pascal'
    print(language)

    s1 = 'C++'
    s2 = 'Python'
    s3 = 'Java'
    s3 = s2
    s1 = s3

---

## Переменный

    name = "Jakhongir"

    a = 7
    a = 5
    print(a)
    
    b = a
    print(a, b)

    a = b = c = 0

    a, b = 1, 2

    a, b = b, a

    # types int, float, str
    x = "hello"
    z = 1.6
    print(type(x), type(z))

+ noun, a-z, A-Z, _, 0-9
+ reserved words True, False, bool, print, input, functions, max, min and etc
+ cmd help -> keywords

HW

    input name, age
    print(name, age)

    # print with radius, pi, circle
    Radius 5 equal & circle surface = 78.75

---

## Типы данных

### Integer & float

    int : 1, -7, 93, ...
    float : 2.5, 1.6, -4.3, ...    !important .

    # comfortable
    population = 35_300_000

    input(int())

    +, -, *, /, //,  **, %, 

    # read all operations from left to right except **
    2 ** 3 ** 2 = 512
    
    # priority
    (), **, *, /, +, -

    27 ** 1/3

    # equal
    i = 2
    j = 5
    i = i + 1
    i += 1
    j -= 2
    
    # modul, min, max , pow, round,
    abs(-3) = 3  
    min(1, 3, 54, 23, 21, 7, ...)
    max(1, 3, 54, 23, 21, 7, ...)
    pow(2, 3) = 2 ** 
    round(3.5) = 3 or 4

HW

    # cout age (byear - current year)
    
    a ^ 2 
    a ^ 3

    # math all operations with f-string
    
    -7, -10, -3 = -20

    # Объём куба и площадь полной поверхности можно вычислить по формулам V = a^3, S = 6a^2

    1 = after 1 next number is 2, before 1 number is 0

---

### String

    # spatial syntax \n, \t
    
    a = "4", 'python', '''I love Python'''
    print(type(a))

    # format
    txt1 = "My name is {fname}, I'm {age}".format(fname = "John", age = 36)
    txt2 = "My name is {0}, I'm {1}".format("John",36)
    txt3 = "My name is {}, I'm {}".format("John",36)

    # f-string
    print(f"My name is {name}")

    emoji = "🤪"
    
    # add func concatenation (конкатенация)
    print("My name is " + name)

    # multiply duplication (дубликация)
    'xa ' * 3

    # compare
      лес > лис

    # methods
    len(), .upper(), .lower(), title(), .capitalize()

    'xyz' in 'abcdefghijklmnopqrstuvwxyz'

    .lstrip(), .rstrip(), .strip() 
    fruict = '  apple   '

    name = input(str('Enter your name:'))
    print(name.Capitalize())

HW

    # input & f-string
    Country: Uzbekistan, region:    navoi, STREET: NAVOI, 
    Apartment: 21 

    # output str and get str
    -1 = -1 , 0, 1

+ In coding all start from 0, not from 1
  <img src="./materials/ASCII.jpg" alt="">

---

### Boolean & операторы сравнение

    4 > 5
    4 <= 5

    a, b = 3, 5
    res = a > b
    print(type(res))

    x = 4
    x == 4
    23 != 23

    # Error 
    =!, =>, =<

    # четное или нечетное
    x = 2, 4, 6, ...
    x % 2 == 0

    # between x and/or  y
    y = 1.6
    y >= -3 and y <= 7
    y < -3 or y > 7

    # not
    not(2 > 0 or 8 < 10)

    # priority not, and, or

    # empty == False, smth == True

    