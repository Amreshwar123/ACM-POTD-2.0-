import sys

def main():
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    m = int(input_data[1])
    
    turned_on = set()
    idx = 2
    
    for _ in range(n):
        x = int(input_data[idx])
        idx += 1
        for _ in range(x):
            turned_on.add(int(input_data[idx]))
            idx += 1
            
    if len(turned_on) == m:
        print("YES")
    else:
        print("NO")

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/07-11-2026.png
