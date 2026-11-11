import sys

def solve():
    # Read all inputs from standard input at once for speed
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    a = [int(x) for x in input_data[1:]]
    
    if n == 0:
        print(0)
        return

    max_len = 1
    curr_len = 1

    for i in range(1, n):
        if a[i] > a[i - 1]:
            curr_len += 1
        else:
            max_len = max(max_len, curr_len)
            curr_len = 1  # Reset for the new sequence

    # Final check for the last running sequence
    max_len = max(max_len, curr_len)

    print(max_len)

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/11-11-2026.png
