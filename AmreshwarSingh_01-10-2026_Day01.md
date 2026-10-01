import sys

def solve():
    # Read all inputs from standard input
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    m = int(input_data[1])
    grid = input_data[2:]
    
    min_row, max_row = n, -1
    min_col, max_col = m, -1
    
    # Find the bounding box limits containing '*'
    for i in range(n):
        for j in range(m):
            if grid[i][j] == '*':
                if i < min_row: min_row = i
                if i > max_row: max_row = i
                if j < min_col: min_col = j
                if j > max_col: max_col = j
                
    # Print the cropped sub-grid
    for i in range(min_row, max_row + 1):
        print(grid[i][min_col:max_col + 1])

if __name__ == '__main__':
    solve()

URL:https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/01-10-2026.png
