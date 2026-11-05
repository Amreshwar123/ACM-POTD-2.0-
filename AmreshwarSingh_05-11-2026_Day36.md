import sys


def main():
    # Read k, n, w from input
    k, n, w = map(int, sys.stdin.read().split())

    # Calculate total cost using the arithmetic progression sum formula
    total_cost = k * w * (w + 1) // 2

    # Amount needed to borrow
    borrow = total_cost - n

    # Print answer (0 if soldier already has enough money)
    print(max(0, borrow))


if __name__ == "__main__":
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/05-11-2026.png
