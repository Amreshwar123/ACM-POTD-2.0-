def decode_borze():
    s = input().strip()
    result = []
    i = 0
    n = len(s)
    
    while i < n:
        if s[i] == '.':
            result.append('0')
            i += 1
        elif s[i] == '-':
            if i + 1 < n and s[i + 1] == '.':
                result.append('1')
            else:
                result.append('2')
            i += 2
            
    print("".join(result))

if __name__ == '__main__':
    decode_borze()

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/05-10-2026.png
