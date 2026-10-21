import sys

def solve():
    # Read all input from standard input
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    m = int(input_data[1])
    rows = input_data[2:]
    
    for i in range(n):
        # Condition 1: All characters in the current row must be the same
        if len(set(rows[i])) != 1:
            print("NO")
            return
        
        # Condition 2: Adjacent rows must not have the same color
        if i < n - 1 and rows[i][0] == rows[i + 1][0]:
            print("NO")
            return
            
    print("YES")

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/02-10-2026.png
