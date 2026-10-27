import sys

def solve():
    # Read all inputs from standard input
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    
    # Sum of the n-1 watched episodes provided in the input
    watched_sum = sum(int(x) for x in input_data[1:])
    
    # Total sum of numbers from 1 to n using the formula n * (n + 1) / 2
    total_sum = n * (n + 1) // 2
    
    # The missing episode is the difference between the total sum and the watched sum
    print(total_sum - watched_sum)

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/27-10-2026.png
