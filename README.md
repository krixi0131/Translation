# Translation
```python
a=str(input())
b=str(input())
c=[]
for i in range(len(a)-1,-1,-1):
    c.append(a[i])
check=0
if len(b)!=len(c):
    check=1
    print("NO")
    exit(0)
for i in range(len(a)):
    if b[i]!=c[i]:
        check=1
if check==1:
    print("NO")
else:
    print("YES")
```
