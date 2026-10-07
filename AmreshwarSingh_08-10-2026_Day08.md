import sys


def solve():
  s = sys.stdin.readline().strip()
  t = sys.stdin.readline().strip()

  # Check if t is the reverse of s
  if s == t[::-1]:
    print("YES")
  else:
    print("NO")


if __name__ == "__main__":
  solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/08-10-2026.png
