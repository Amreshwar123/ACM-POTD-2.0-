import sys

def main():
    input = sys.stdin.read
    data = input().split()
    if not data:
        return
    
    n = int(data[0])
    values = [int(x) for x in data[1:]]
    
    # Create pairs of (value, 1-based index)
    cards = [(values[i], i + 1) for i in range(n)]
    
    # Sort by card value
    cards.sort(key=lambda x: x[0])
    
    # Pair smallest with largest
    for i in range(n // 2):
        print(f"{cards[i][1]} {cards[n - 1 - i][1]}")

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/10-11-2026.png
