import sys

def solve():
    n = int(sys.stdin.read().strip())
    if n % 2 == 0:
        print(f"8 {n - 8}")
    else:
        print(f"9 {n - 9}")

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/01-11-2026.png
