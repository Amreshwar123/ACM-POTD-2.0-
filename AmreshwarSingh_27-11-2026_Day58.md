#include <stdio.h>

int main(void) {
    int n, k;
    if (scanf("%d %d", &n, &k) != 2) {
        return 0;
    }

    char road[300005];
    scanf("%300004s", road);

    int consecutive_rocks = 0;
    for (int i = 0; i < n; i++) {
        if (road[i] == '#') {
            consecutive_rocks++;
            if (consecutive_rocks >= k) {
                printf("NO\n");
                return 0;
            }
        } else {
            consecutive_rocks = 0;
        }
    }

    printf("YES\n");
    return 0;
}

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/27-11-2026.png
