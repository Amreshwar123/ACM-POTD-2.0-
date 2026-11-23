import sys

def solve():
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    # Count frequencies directly from the sliced input
    arr = input_data[1:n+1]
    
    c1 = arr.count('1')
    c2 = arr.count('2')
    c3 = arr.count('3')
    
    print(n - max(c1, c2, c3))

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/21-11-2026.png
