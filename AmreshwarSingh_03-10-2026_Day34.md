import sys

def main():
    n = int(sys.stdin.read())
    
    height = 0
    current_level_cubes = 0
    
    while True:
        height += 1
        current_level_cubes += height
        if n >= current_level_cubes:
            n -= current_level_cubes
        else:
            height -= 1
            break
            
    print(height)

if __name__ == '__main__':
    main()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/03-11-2026.png
