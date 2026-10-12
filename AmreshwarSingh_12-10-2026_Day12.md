s = input()
upper_count = 0

for x in s:
    if x.isupper():
        upper_count += 1

if upper_count > len(s) // 2:
    print(s.upper())
else:
    print(s.lower())

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/12-10-2026.png
