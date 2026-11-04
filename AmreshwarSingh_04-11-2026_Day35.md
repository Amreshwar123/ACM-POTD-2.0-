import sys

def main():
    n = int(sys.stdin.readline())
    s = sys.stdin.readline().strip()

    # Convert to lowercase and find unique characters using a set
    unique_letters = set(s.lower())

    # Check if the count of unique letters is 26
    if len(unique_letters) == 26:
        print("YES")
    else:
        print("NO")

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/04-11-2026.png
