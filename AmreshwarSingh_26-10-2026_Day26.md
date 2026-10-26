import sys

def solve():
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    n = int(input_data[0])
    s = int(input_data[1])
    m = [int(x) for x in input_data[2:]]
    
    # Sort mugs to find the smallest n-1 mugs
    m.sort()
    
    # Check if the sum of the first n-1 mugs exceeds s
    if sum(m[:n-1]) <= s:
        print("YES")
    else:
        print("NO")

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/26-10-2026.png
