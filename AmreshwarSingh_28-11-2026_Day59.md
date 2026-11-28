#include <stdio.h>

int main(void) {
    long long n, k;
    if (scanf("%lld %lld", &n, &k) != 2) {
        return 0;
    }

    long long odd_count = (n + 1) / 2;

    if (k <= odd_count) {
        printf("%lld\n", 2 * k - 1);
    } else {
        printf("%lld\n", 2 * (k - odd_count));
    }

    return 0;
}

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/28-11-2026.png
