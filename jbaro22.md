# Profile: Jil Barot

- **NetID:** jbaro22
- **Major:** Computer Science
- **Question that I chose from the memoization exercise:** Ways to Climb Stairs Without Considering Order
- **Link to the question article:** [(https://www.geeksforgeeks.org/problems/count-ways-to-nth-stairorder-does-not-matter5639/1?utm_source=geeksforgeeks&utm_medium=article_practice_tab&utm_campaign=article_practice_tab)]

## My Solution

```c
#include <stdio.h>

int nthStair(int n) {

    // We can take either 1 or 2 stairs at a time.
    // Since order does not matter, we only count
    // the possible number of 2-step moves.

    // For example, n = 4:
    // 1 + 1 + 1 + 1
    // 1 + 1 + 2
    // 2 + 2
    // Total = 3 ways

    return (n / 2) + 1;
}

int main(void) {
    int n;

    scanf("%d", &n);

    printf("%d\n", nthStair(n));

    return 0;
}
```
