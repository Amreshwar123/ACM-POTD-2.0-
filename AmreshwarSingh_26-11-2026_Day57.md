#include <stdio.h>

int main(void) {
    int presses[3][3];
    int dr[4] = {-1, 1, 0, 0};
    int dc[4] = {0, 0, -1, 1};

    for (int r = 0; r < 3; r++) {
        for (int c = 0; c < 3; c++) {
            scanf("%d", &presses[r][c]);
        }
    }

    for (int r = 0; r < 3; r++) {
        for (int c = 0; c < 3; c++) {
            int total = presses[r][c];
            for (int k = 0; k < 4; k++) {
                int nr = r + dr[k];
                int nc = c + dc[k];
                if (nr >= 0 && nr < 3 && nc >= 0 && nc < 3) {
                    total += presses[nr][nc];
                }
            }
            /* Starts ON (1); flips to OFF (0) if total toggles is odd */
            printf("%d", (total % 2 == 0) ? 1 : 0);
        }
        printf("\n");
    }

    return 0;
}

https://github.com/Amreshwar123/ACM-POTD-2.0-/blob/main/26-11-2026.png
