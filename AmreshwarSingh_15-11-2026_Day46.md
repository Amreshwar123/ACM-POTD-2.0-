import sys

def main():
    # Read all inputs from standard input efficiently
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    # Parse the 4 segment lengths and sort them
    arr = [int(x) for x in input_data[:4]]
    arr.sort()
    
    # Check for a non-degenerate triangle
    # If the sum of any two smaller sides is strictly greater than the largest of the 3
    if arr[0] + arr[1] > arr[2] or arr[1] + arr[2] > arr[3]:
        print("TRIANGLE")
    # Check for a degenerate triangle (collinear points forming a segment)
    elif arr[0] + arr[1] == arr[2] or arr[1] + arr[2] == arr[3]:
        print("SEGMENT")
    # Otherwise, it's impossible
    else:
        print("IMPOSSIBLE")

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/15-11-2026.png
