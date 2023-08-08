# T-o-Lao
Đăng các code cần nhớ thông qua notion
// phân tích thừa số nguyên tố
def temp():
    a = [2, 3]
    for i in range(4, 100):
        for j in a:
            if i % j == 0:
                break
        else:
            a.append(i)
    return a

def main():
    n = int(input())
    arr_kq = []
    for i in temp():
        while n % i == 0:
            arr_kq.append(i)
            n //= i
    if n > 1:
        arr_kq.append(n)
    for i in arr_kq:
        print(i, end=" ")

if __name__ == "__main__":
    main()

