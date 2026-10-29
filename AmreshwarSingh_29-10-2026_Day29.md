import sys

def solve():
    n = int(sys.stdin.read().strip())
    
    d_count = 1
    for i in range(n):
        stars = (n - d_count) // 2
        print("*" * stars + "D" * d_count + "*" * stars)
        
        if i < n // 2:
            d_count += 2
        else:
            d_count -= 2

if __name__ == "__main__":
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/29-10-2026.png
