Function definitions
====================
custom functions
----------------
````ruby
def draw_triangle(fill, base):

    for i in range(base // 2):
        print(fill * (i + 1))

    for i in range(base // 2, -1, -1):
        print(fill * (i + 1))
fill = input()
base = int(input())
draw_triangle(fill, base)
````
````ruby
def print_digit_sum(num):
    cnt = 0
    while num != 0:
        cnt += num % 10
        num = num//10
    print (cnt)
n =int(input())
print_digit_sum(n)
````
