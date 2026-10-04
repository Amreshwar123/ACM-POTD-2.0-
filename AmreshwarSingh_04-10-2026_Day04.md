def solve():
    # Read n and d
    n, d = map(int, input().split())
    # Read the heights of the soldiers
    a = list(map(int, input().split()))
    
    count = 0
    # Check all possible pairs (i, j) where i != j
    for i in range(n):
        for j in range(n):
            if i != j and abs(a[i] - a[j]) <= d:
                count += 1
                
    print(count)

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/04-10-2026.png
