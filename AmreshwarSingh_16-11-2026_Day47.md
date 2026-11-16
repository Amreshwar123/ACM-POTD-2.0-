import sys


def solve():
  # Read all inputs from standard input efficiently
  input_data = sys.stdin.read().split()
  if not input_data:
    return

  n = int(input_data[0])
  d = int(input_data[1])
  a = [int(x) for x in input_data[2:]]

  total_operations = 0

  for i in range(1, n):
    if a[i] <= a[i - 1]:
      # Calculate the difference and the number of operations needed
      diff = a[i - 1] - a[i]
      ops = (diff // d) + 1

      # Update the current element and the total operation counter
      a[i] += ops * d
      total_operations += ops

  print(total_operations)


if __name__ == "__main__":
  solve()

github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/16-11-2026.png
