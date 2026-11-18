import sys

n = int(sys.stdin.read())
f = [0] * (n + 1)

for i in range(2, n + 1):
    if f[i] == 0:
        for j in range(i, n + 1, i):
            f[j] += 1

print(f.count(2))

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/18-11-%202026.png
