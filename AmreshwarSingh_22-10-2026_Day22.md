import sys

def main():
    # Read n from standard input
    n = int(sys.stdin.read().strip())
    
    # Calculate the maximum number of coders (ceil(n^2 / 2))
    max_coders = (n * n + 1) // 2
    print(max_coders)
    
    # Generate and print the chessboard configuration
    for i in range(n):
        row = []
        for j in range(n):
            # If (i + j) is even, place a Coder, otherwise an empty cell
            if (i + j) % 2 == 0:
                row.append('C')
            else:
                row.append('.')
        print(''.join(row))

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/22-10-2026.png
