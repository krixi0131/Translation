# Translation
The translation from the Berland language into the Birland language is not an easy task. Those languages are very similar: a berlandish word differs from a birlandish word with the same meaning a little: it is spelled (and pronounced) reversely. For example, a Berlandish word code corresponds to a Birlandish word edoc. However, it's easy to make a mistake during the «translation». Vasya translated word s from Berlandish into Birlandish as t. Help him: find out if he translated the word correctly.

Input
The first line contains word s, the second line contains word t. The words consist of lowercase Latin letters. The input data do not consist unnecessary spaces. The words are not empty and their lengths do not exceed 100 symbols.

Output
If the word t is a word s, written reversely, print YES, otherwise print NO.
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
