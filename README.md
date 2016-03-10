# Codility Tests

* [CyclicRotation](https://codility.com/demo/results/trainingASEHVN-7VQ/)
Rotate an array to the right by a given number of steps.

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

* [OddOccurrencesInArray](https://codility.com/demo/results/trainingGZAR3J-BPH/)
Find value that occurs in odd number of elements.

```python
def solution(A):
    for value in list(set(A)):
        if A.count(value) == 1:
            return value
```
