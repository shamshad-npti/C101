#Copy Array
Write a program to copy content of array `a` to array `b`.

**Description**: Given two array `a` and `b`, let `a[] = {2, 4, 5, 6}` and `b` is unknown. When we execute copy operation - `a` 
would be unchanged but content of `b` would be {2, 4, 5, 6}.

**Task** - Complete following copy function (Assume that size of `b` is always larger than that of `a`):

```C
void copy(int* a, int* b, int size) {
    int i;
    for(i = 0; i < size; i++) {
        b[i] = a[i];
    }
}
```

** How full program looks like **
```C
#include <stdio.h>

void copy(int *a, int* b, int size) {
    int i;
    for(i = 0; i < size; i++) {
        b[i] = a[i];
    }
}

void main() {
    int a[10], b[10], size, i;
    printf("Enter size of the array:");
    scanf("%d", &size);
    printf("Enter elements in array:");
    for(i = 0; i < size; i++) {
        scanf("%d", &a[i]);
    }
    copy(a, b, size);
    printf("Elements in b after copy:\n");
    for(i = 0; i < size; i++) {
        printf("%d ", b[i]);
    }
}
```
