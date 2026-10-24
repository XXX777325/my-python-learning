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

# 给定整数n后，编写一个程序生成包含（i， i*i）且 是介于1和n之间的整数（两者均包含）的字典。然后程序应该打印字典。 假设向程序提供了以下输入： 8 那么，输出应为： {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}
q1 = int(input('请输入数字：'))
answer = dict()
for i in range(1,q1+1):
  answer[i] = i*i
print(answer)

#编写一个程序，接受控制台中逗号分隔的数字序列，生成包含所有数字的列表和元组。 假设向程序提供了以下输入： 34,67,55,33,12,98 那么，输出应为： ['34', '67', '55', '33', '12', '98'] ('34', '67', '55', '33', '12', '98')
q1 = input('请输入数字：')
print(list(q1.split(',')),tuple(q1.split(',')))

#定义一个至少有两个方法的类： getString： 从控制台输入获取字符串 printString：用于打印大写字符串。 还请包含简单的测试函数来测试类方法。
class transform :
  def _init_(self):
    s = ''
  def getString(self) :
    self.s = input()
  def printString(self) :
    print(self.s.upper())
tran = transform()
tran.getString()
tran.printString()

#素数指的是只能被 1 和自身整除的正整数（不包括 1），之前我们写过判断素数的代码，这里相当于是一个升级版本。
num = int(input('请输入数字')
for i in range(0,num+1) :
    if all(i%j!= 0 for J in range(2,i)):
        print(i)
#埃拉托斯特尼筛法（找"范围内所有素数"最快）
num = int(input('请输入数字'))
is_prime = [True] * (num + 1)
is_prime[0] = is_prime[1] = False

for i in range(2, int(num ** 0.5) + 1):
    if is_prime[i]:
        for j in range(i * i, num + 1, i):
            is_prime[j] = False

for i in range(2, num + 1):
    if is_prime[i]:
        print(i)
输出斐波那契数列中的前 20 个数
a = 1 
b = 1
print(a)
print(b)
for i in range(0,19) :
    if a<=b:
        a = a+b
        print(a)
    else :
        b = a+b
        print(b)
    #编写一个程序，按照给定公式计算并打印该值： Q = [（2 * C * D）/H] 的平方根 以下是C和H的固定值： C是50。H是30岁。 D 是应以逗号分隔序列输入程序的变量。 示例 假设程序给出以下逗号分隔的输入序列： 100,150,180 程序输出应为： 18,22,24
num = input("请输入逗号分隔的输入序列：")
num = num.split(",")
num1 = []
for i in num:
    i = int(i)
    num1.append(int(((2 * 50 * i) / 30)**0.5))
print(",".join(map(str,num1)))
    

在开始本节课的内容之前，我们先给大家一个编程任务，将一颗色子掷 6000 次，统计每种点数出现的次数。这个任务对大家来说应该是非常简单的，我们可以用 1 到 6 均匀分布的随机数来模拟掷色子，然后用 6 个变量分别记录每个点数出现的次数
import random
counts = [0]*7
for i in range(1,6001):
    point = random.randint(1,6)
    counts[point] +=1
for i in range(1,7):
    print(f'{i}出现{counts[i]}次')










