```C
void copy(int *a, int *b, int *c, int size_a, int size_b) {
    int i, j;
    for(i = 0; i < size_a; i++) {
        c[i] = a[i];
    }
    for(i = 0, j = size_a; i < size_b; i++, j++) {
        c[j] = b[i];
    }
}

void main() {
    int a[10], b[5], c[15];
    //...
    copy(a, b, c, 10, 5);
    //...
}
```
