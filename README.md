# Codility Tests

* [CyclicRotation](https://codility.com/demo/results/trainingASEHVN-7VQ/)

```python
def solution(A, K):
    B = []
    if len(A) < 2:
        return A

    while K > len(A):
        K -= len(A)

    for i in range(0, len(A)):
        B.append(A[i-K])
    return B
```
