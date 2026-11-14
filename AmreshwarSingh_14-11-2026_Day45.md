n = int(input())
s = input().strip()

anton = s.count('A')
danik = n - anton

if anton > danik:
    print("Anton")
elif danik > anton:
    print("Danik")
else:
    print("Friendship")

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/14-11-2026.png
