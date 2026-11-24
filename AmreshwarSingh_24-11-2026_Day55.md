#include <stdio.h>
#include <stdlib.h>

static int cmp_desc(const void *lhs, const void *rhs) {
    int a = *(const int *)lhs;
    int b = *(const int *)rhs;
    if (a < b) return 1;
    if (a > b) return -1;
    return 0;
}

int main(void) {
    int n, k;
    if (scanf("%d %d", &n, &k) != 2) {
        return 0;
    }

    int a[50];
    for (int i = 0; i < n; ++i) {
        if (scanf("%d", &a[i]) != 1) {
            return 0;
        }
    }

    if (k > n) {
        printf("-1\n");
        return 0;
    }

    qsort(a, (size_t)n, sizeof(int), cmp_desc);
    printf("%d 0\n", a[k - 1]);

    return 0;
}

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/24-11-2026.png
