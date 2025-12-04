#1
minutes = int(input("Введите минуты:"))
hours = minutes // 60
remaininng_minutes = minutes % 60

print(f"{hours}")
print(f"{remaininng_minutes}")

#2
a = int(input())
b = int(input())
h = int(input())

if h < a:
    print("Недосып")
elif h > b:
    print("Пересып")
else:
    print("Это нормально")

#3
d = float(input())
f = float(input())
g = float(input())

p = (d + f + g) / 2
s = (p * (p-d) * (p-f) * (p-g)) ** 0.5
print(s)

#4
figure = input()

if figure == "треугольник":
    a = float(input())
    b = float(input())
    c = float(input())
    p = (a + b + c) / 2
    s = (p * (p-a) * (p-b) * (p-c)) ** 0.5
elif figure == "прямоугольник":
    a = float(input())
    b = float(input())
    s = a * b
elif figure == "круг":
    r = float(input())
    s = 3.14 * r ** 2
print(s)
#5
n = int(input())
last_digit = n % 10
last_two_digits = n % 100

if 11 <= last_two_digits <= 14:
    ending = "программистов"
elif last_digit == 1:
    ending = "программист"
elif 2 <= last_digit <= 4:
    ending = "программиста"
else:
    ending = "программистов"

print(n, ending)
#6
ticket = input()

if len(ticket) != 6:
    print("Неверный ввод")
else:
    sum1 = int(ticket[0]) + int(ticket[1]) + int(ticket[2])
    sum2 = int(ticket[3]) + int(ticket[4]) + int(ticket[5])

  if sum1 == sum2:
        print("Счастливый")
   else:
        print("Обычный")    
