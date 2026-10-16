n, m = map(int, input().split())
count = 0

for a in range(1001):
    for b in range(1001):
        if a**2 + b == n and a + b**2 == m:
            count += 1

print(count)

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/16-10-2026.png
