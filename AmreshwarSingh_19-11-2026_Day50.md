import sys

def solve():
    data = sys.stdin.read().split()
    if not data:
        return
    
    n = int(data[0])
    m = int(data[1])
    prices = [int(x) for x in data[2:2 + n]]
    
    # Filter negative prices, sort most negative first, and take up to m
    negative_prices = sorted(p for p in prices if p < 0)
    max_earnings = -sum(negative_prices[:m])
    
    print(max_earnings)

if __name__ == "__main__":
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/19-11-2026.png
