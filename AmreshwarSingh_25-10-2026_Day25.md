n, a, b = map(int, input().split())
arthur = set(map(int, input().split()))
alexander = set(map(int, input().split()))

result = []
for i in range(1, n + 1):
    if i in arthur:
        result.append(1)
    else:
        result.append(2)

print(*result)

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/25-10-2026.png
