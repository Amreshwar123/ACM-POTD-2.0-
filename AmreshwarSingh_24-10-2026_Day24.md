import sys


def solve():
    s = sys.stdin.readline().strip()

    # Check all conditions:
    # 1. Length is at least 5
    # 2. Contains at least one uppercase letter (large English letter)
    # 3. Contains at least one lowercase letter (small English letter)
    # 4. Contains at least one digit

    if (
        len(s) >= 5
        and any(c.isupper() for c in s)
        and any(c.islower() for c in s)
        and any(c.isdigit() for c in s)
    ):
        print("Correct")
    else:
        print("Too weak")


if __name__ == "__main__":
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/24-10-2026.png
