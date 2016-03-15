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

* [OddOccurenciesInArray](https://codility.com/demo/results/trainingZ38Y5B-Y5R/)

```python
def solution(A):
    count = {}
    for i in A:
        count[i] = count.get(i, 0) + 1
        
    for val in count.values():
        if val % 2 != 0:
            return count.keys()[count.values().index(val)]
```

* [FrogJmp](https://codility.com/demo/results/trainingN9HEWR-449/)

```python
def solution(X, Y, D):
    res = int(round((Y - X) / float(D)))
    if res*D + X < Y:
        res += 1
    return res
```
