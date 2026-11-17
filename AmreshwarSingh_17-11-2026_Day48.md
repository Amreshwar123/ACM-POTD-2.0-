import sys

def solve():
    input_data = sys.stdin.read().split()
    if not input_data:
        return
    
    n = int(input_data[0])
    m = int(input_data[1])
    
    containers = []
    idx = 2
    for _ in range(m):
        a = int(input_data[idx])
        b = int(input_data[idx + 1])
        containers.append((b, a))
        idx += 2
        
    # Sort by matches per box (b_i) in descending order
    containers.sort(reverse=True)
    
    total_matches = 0
    for matches_per_box, boxes in containers:
        if n == 0:
            break
        take = min(n, boxes)
        total_matches += take * matches_per_box
        n -= take
        
    print(total_matches)

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/17-11-2026.png
