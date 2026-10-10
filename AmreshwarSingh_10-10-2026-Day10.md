import sys


def solve():
    # Read all input from standard input and remove surrounding whitespace
    s = sys.stdin.read().strip()

    # Traverse backwards to find the last alphabetical character
    for char in reversed(s):
        if char.isalpha():
            # Check if the last letter is a vowel (including 'y')
            if char.lower() in {"a", "e", "i", "o", "u", "y"}:
                print("YES")
            else:
                print("NO")
            return


if __name__ == "__main__":
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/10-10-2026.png
