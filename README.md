# T-o-Lao
Đăng các code cần nhớ thông qua notion
// hàm sơ khai của phân tích thừa số nguyên tố
import math
def temp():
    a = []
    a.append(2)
    a.append(3)
    for i in range(4,100):
        haha = int(math.sqrt(i))
        cnt = 0
        for j in range(2,haha+1):
            if i %j == 0:
                cnt+=1
                break
        if cnt == 0:
            a.append(i)
    return a
arr_nt = temp()
n = int(input())
arr_kq = []
dem = 0
while n != 1:
    while n % arr_nt[dem] == 0:
        arr_kq.append(arr_nt[dem])
        n //= arr_nt[dem]
    if n % arr_nt[dem] != 0:
        dem+=1
for i in arr_kq:
    print(i,end=" ")

