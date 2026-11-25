#include <stdio.h>

int main(void) {
    int n;
    if (scanf("%d", &n) != 1) {
        return 0;
    }

    while (n--) {
        long long a, b;
        scanf("%lld %lld", &a, &b);

        long long ops = 0;
        while (a > 0 && b > 0) {
            if (a < b) {
                long long tmp = a;
                a = b;
                b = tmp;
            }
            ops += a / b;
            a %= b;
        }

        printf("%lld\n", ops);
    }

    return 0;
}

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/25-11-2026.png
