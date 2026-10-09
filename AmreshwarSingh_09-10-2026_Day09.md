n = int(input())

k = 1
while True:
    triangular = (k * (k + 1)) // 2
    if triangular == n:
        print("YES")
        break
    elif triangular > n:
        print("NO")
        break
    k += 1

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/09-10-2026.png
