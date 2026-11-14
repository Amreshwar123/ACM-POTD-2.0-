# Codeforces 710A - King Moves
# Language: Python 3

import sys

def main():
    # Read the input string from standard input
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    s = input_data[0]
    col = s[0]
    row = s[1]
    
    # Condition 1: Corner squares have only 3 valid moves
    if (col == 'a' or col == 'h') and (row == '1' or row == '8'):
        print(3)
    # Condition 2: Edge squares (non-corner) have 5 valid moves
    elif col == 'a' or col == 'h' or row == '1' or row == '8':
        print(5)
    # Condition 3: Interior squares have all 8 valid moves
    else:
        print(8)

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/13-11-2026.png
