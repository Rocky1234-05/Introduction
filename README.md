# Introduction
I’m a Grade 12 student at an international high school, where I’ve consistently achieved strong academic results. In addition to my studies, I’m passionate about sports, particularly golf. I’ve had the opportunity to compete in various tournaments, earning several awards along the way. Balancing academics and athletics has taught me discipline and time management, and I look forward to continuing to excel in both areas as I prepare for the future.
Looking forward to meet with you guys.

# a => variable 变量
# 5 -》 value 值
# assign 5 as the value to variable a
a = 5
b = 3
c = a + b
d = a - b
e = a * b
# 除法
f = a / b
# 整数，只有整数，丢掉小数
g = a // b
print(f)
print(g)
# mod，求余数
h = a % b
print(h)


number = 3

if number > 0:
    print("number bigger 0")
else:
    print("number smaller equals 0")
    
# 判断相等
if number == 0:
    print("number bigger 0")
else:
    print("number smaller equals 0")

# 判断不相等
if number != 0:
    print("number bigger 0")
else:
    print("number smaller equals 0")



number = 10
 # and => 条件都满足的情况下
 if number > 5 and number % 2 ==0:
    print("number 是一个大于5的偶数")
    
# or => 满足任意条件即可
 if number > 5 or number % 2 ==0:
    print("number 是一个大于5的数字或者是一个偶数")


# for loop
# range里如果只有一个数字，默认从0开始，左闭右开
# 每循环一次，i会自动加1
# for i in range(10):
#     print(i)

# 求1加到10的累加和是多少，1+2+3+4+....+10
total = 0
for i in range(1, 11):
    total = total + i
print(total)

# 打印10以内所有的偶数
for i in range(11):
    if i % 2 == 0:
        print(i)


# 判断一个数字是不是质数
# 解题思路：判断有没有factor，除了1和自己以外都不可以整数
# it is prime / it is not prime

number = 10
hasFactor = 0
for i in range(2, number):
    if number % i == 0:
        hasFactor = 1

if hasFactor == 0:
    print("it is prime")
else:
    print("it is not")


# sum from 1 to 100
# i = 1
# total = 0
# while i <= 100:
#     total += i
#     i += 1
# print(total)
#
# number = 10

# i是自然数
i = 1
while i <= 100:
    # 检查当前数字i是不是质数
    hasFactor = 0
    j = 2
    while j < i:
        if i % j == 0:
            hasFactor = 1
        j += 1

    if hasFactor == 0:
        print(i)
    i += 1


# for loop
# range里如果只有一个数字，默认从0开始，左闭右开
# 每循环一次，i会自动加1
# for i in range(10):
#     print(i)

# 求1加到10的累加和是多少，1+2+3+4+....+10
# total = 0
# for i in range(1, 11):
#     total = total + i
# print(total)

# 打印10以内所有的偶数
# for i in range(11):
#     if i % 2 == 0:
#         print(i)

# 判断一个数字是不是质数
# 解题思路：判断有没有factor，除了1和自己以外都不可以整数
# it is prime / it is not prime
number = 10
hasFactor = 0
for i in range(2, number):
    if number % i == 0:
        hasFactor = 1
if hasFactor == 0:
    print("it is prime")
else:
    print("it is not")

# 打印某一个数字的所有的约数
for i in range(1, number + 1):
    if number % i == 0:
        print(i)

# print all prime number under 100
for i in range(1, 101):
    # check the current is prime or not
    hasFactor = 0
    for j in range(2, i):
        if i % j == 0:
            hasFactor = 1
    if hasFactor == 0:
        print(i)


# 目标
s = 4.3
# 游了几步
steps = 0
# 当前这一步游了多远
current = 2
# 已经游了多远
total = 0
while total < s:
    # 每游一次，步数加一
    steps += 1
    # 记录游了多远
    total += current
    # 是上一步的0.98
    current *= 0.98
print(steps)


n = 5
# 阶乘和
total = 0
# 代表每一个数字
for i in range(1, n + 1):
    # 当前数字的阶乘
    factorial = 1
    for j in range(1, i + 1):
        factorial *= j
    total += factorial
print(total)



numbers = [4, 2, 1, 9, 10]

# len方法是求列表的个数
n = len(numbers)

# 通过下标index获得对应的元素，下标从0开始
print(numbers[3])

\

# 打印numbers里所有的质数
for i in range(0, n):
    # 判断当前这个数字是不是质数 numbers[i]
    hasFactor = 0
    for j in range(2, numbers[i]):
        if numbers[i] % j == 0:
            hasFactor = 1
    if hasFactor == 0:
        print(numbers[i])

n = 6
fish = [4, 3, 0, 5, 1, 2]
# 计算自己的左边有几个比自己小的数字，依次打印
# 最终输出的结果：0，0，0，3，1，2

for i in range(0, n):
    counter = 0
    for j in range(0, i):
        if fish[j] < fish[i]:
            counter += 1
    print(counter)