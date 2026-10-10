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

