def solve():
    n = int(input())
    # Generate alternating layers, join with " that ", and append " it"
    layers = ["I hate" if i % 2 != 0 else "I love" for i in range(1, n + 1)]
    print(" that ".join(layers) + " it")

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/12-11-2026.png
