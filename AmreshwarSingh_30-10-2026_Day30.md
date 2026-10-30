def solve():
    rooms_count = int(input())
    available_rooms = 0
    
    for _ in range(rooms_count):
        p, q = map(int, input().split())
        # Check if the room has space for both George and Alex
        if q - p >= 2:
            available_rooms += 1
            
    print(available_rooms)

if __name__ == '__main__':
    solve()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/30-10-2026.png
