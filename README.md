# my-python-learning
I hope everyone is doing OK.
#day 10.10
#输入华氏温度将其转换为摄氏温度，华氏温度到摄氏温度的转换公式为： c =( F-32)/1.8
F = Fahrenheit = float(input('当前华氏度是：'))
c = (F-32)/1.8
print(f'当前华氏度是{F},摄氏度是{c:.1f}')
#输入一个圆的半径（$\small{r}$），计算出它的周长和面积
import math                             #代码中的import math表示导入math模块，导入该模块以后，才能用math.pi得到圆周率的值。
r = float(input('圆的半径'))
C = 2*math.pi*r
s = math.pi*(r**2)
print(f'该原的周长是{C:.2f},面积是{s:.2f}')
#判断闰年
year = int(input('请输入年份:')
result = year%4 == 0 and year%100 != 0 or year%400 == 0
print(result)

#写一个程序，找出所有能被7整除但不是5的倍数的数字，范围在2000到3200之间（两者都包括在内）。 获得的数字应以逗号分隔的顺序在单行印刷。
for i in range(2000,3201):
  if i%7 == 0 and i%5 != 0 :
    print (i, end=',')

# 编写一个程序，能够计算给定数值的阶乘。 结果应以逗号分隔的顺序单行打印。 假设向程序提供了以下输入： 8 那么，输出应为： 40320
q1 = int(input('请输入数字:'))
result = 1
for i in range(1,q1+1) :  
  result = result*i
print(result)

