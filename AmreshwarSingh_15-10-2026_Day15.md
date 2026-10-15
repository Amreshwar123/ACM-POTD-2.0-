import sys


def solve():
    input = sys.stdin.read
    data = input().split()

    if not data:
        return

    n = int(data[0])
    m = int(data[1])

    grid = data[2:]

    target_row = 0
    target_col = 0

    for i in range(n):
        for j in range(m):
            if grid[i][j] == "*":
                target_row ^= i + 1
                target_col ^= j + 1

    print(f"{target_row} {target_col}")


if __name__ == "__main__":
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/15-10-2026.png
