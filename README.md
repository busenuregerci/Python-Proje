# Python-Proje
l)

[[1,'a',['cat'],2],[[[3]],'dog'],4,5]
def flatten(xs):
    res = []
    def loop(ys):
        for i in ys:
            if isinstance(i, list):
                loop(i)
            else:
                res.append(i)
    loop(xs)
    return res
flatten(l)

[1, 'a', 'cat', 2, 3, 'dog', 4, 5]

2) 

l =[[1, 2], [3, 4], [5, 6, 7]]
l=l[::-1]

for i in range(len(l)):
    (l[i])=(l[i])[::-1]
print(l)

[[7, 6, 5], [4, 3], [2, 1]]
