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
````ruby
def is_prime(num):
    if num == 1:
        return False
    for i in range (2, num):
        if  num % i == 0:
            return False
    else:
        return True

n = int(input())

print(is_prime(n))
````
````ruby
def is_one_away(word1, word2):
    if len(word1) != len(word2):
        return False
    cnt = 0
    for j in range (len(word1)):
        if word1[j] != word2[j] :
            cnt += 1
    if cnt == 0:
        return False
    if cnt >= 2:
        return False
    return True


txt1 = input()
txt2 = input()
 
print(is_one_away(txt1, txt2))
````
````ruby
def is_valid_password(password):
    s = password.split(':')
    if len(s) != 3:
        return False
    flag2 = True
    flag3 = True
    flag4 = True 
    flag5 = True
    if s[0] != s[0][::-1]:
        flag2 = False
    if int(s[1]) == 1:
        flag3 = False
    for i in range (2, (int(s[1])//2)+1):
        if int(s[1]) % i == 0:
            flag4 = False    
    
    if int(s[2])%2 !=0:
        flag5 = False
    if  flag2 == flag3 == flag4 == flag5 == True:
        return True
    else:
        return False

       

psw = input()

print(is_valid_password(psw))
````
