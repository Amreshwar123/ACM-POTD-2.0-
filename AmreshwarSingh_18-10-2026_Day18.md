def solve():
    n = int(input())
    s = input().strip()
    
    ans = 0
    for i in range(1, n):
        if s[i] == s[i - 1]:
            ans += 1
            
    print(ans)

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/18-10-2026.png
