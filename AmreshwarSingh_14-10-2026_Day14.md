# Read n (total participants) and k (place threshold)
n, k = map(int, input().split())

# Read the list of scores
a = list(map(int, input().split()))

# Get the score of the k-th participant (0-indexed, so index is k - 1)
k_score = a[k - 1]

# Count participants who meet the advancement criteria
count = 0
for score in a:
  if score >= k_score and score > 0:
    count += 1

# Print the final count
print(count)

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/14-10-2026.png
