n = int(input())
a = list(map(int, input().split()))

id1, id2 = 1, 2
min_diff = abs(a[0] - a[1])

for i in range(1, n - 1):
    diff = abs(a[i] - a[i + 1])
    if diff < min_diff:
        min_diff = diff
        id1 = i + 1
        id2 = i + 2

# Check wrap-around between last and first element
if abs(a[-1] - a[0]) < min_diff:
    id1, id2 = n, 1

print(id1, id2)

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/06-10-2026.png
