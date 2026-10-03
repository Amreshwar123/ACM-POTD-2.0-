import sys


def solve():
  # Read all inputs from standard input
  input_data = sys.stdin.read().split()
  if not input_data:
    return

  n = int(input_data[0])
  a = list(map(int, input_data[1:]))

  # Remove duplicates using set and sort the unique elements
  unique_sorted = sorted(list(set(a)))

  # If there is a second smallest distinct element, print it
  if len(unique_sorted) > 1:
    print(unique_sorted[1])
  else:
    print("NO")


if __name__ == "__main__":
  solve()


https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/03-10-2026.png
