def solve():
    n = int(input())
    
    # Read player X's levels
    x_input = list(map(int, input().split()))
    p = x_input[0]
    levels_x = x_input[1:]
    
    # Read player Y's levels
    y_input = list(map(int, input().split()))
    q = y_input[0]
    levels_y = y_input[1:]
    
    # Combine both lists into a set to remove duplicates
    passed_levels = set(levels_x + levels_y)
    
    # Check if the number of unique levels equals n
    if len(passed_levels) == n:
        print("I become the guy.")
    else:
        print("Oh, my keyboard!")

if __name__ == '__main__':
    solve()
https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/31-10-2026.png
