import sys

def main():
    n = int(sys.stdin.read().strip())
    if n % 2 == 0:
        print(n // 2)
    else:
        print(-(n + 1) // 2)

if __name__ == '__main__':
    main()
    
    https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/02-11-2026.png
