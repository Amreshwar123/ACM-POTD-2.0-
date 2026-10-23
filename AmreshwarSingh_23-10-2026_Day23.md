import sys

def solve():
    input = sys.stdin.read
    data = input().split()
    if not data:
        return
    
    n = int(data[0])
    bids = [int(x) for x in data[1:n+1]]
    
    max_bid = -1
    winner_idx = -1
    second_max_bid = -1
    
    for i, bid in enumerate(bids, start=1):
        if bid > max_bid:
            second_max_bid = max_bid
            max_bid = bid
            winner_idx = i
        elif bid > second_max_bid:
            second_max_bid = bid
            
    print(f"{winner_idx} {second_max_bid}")

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/23-10-2026.png
