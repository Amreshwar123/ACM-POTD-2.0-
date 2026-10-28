import sys

def main():
    # Read the entire line of input
    s = sys.stdin.readline().strip()
    
    # Extract only the alphabetic characters (a-z) and store them in a set
    distinct_letters = set(c for c in s if 'a' <= c <= 'z')
    
    # The number of distinct letters is the size of the set
    print(len(distinct_letters))

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/28-10-2026.png
