# python-code
python problems 
def f(n):
    x=str(n)
    sum=0
    for i in x:
        fact=1
        for j in range(1,int(i)+1):
            fact=fact*j
        sum+=fact
    return sum 
def sf(n):
    x=str(n)
    sum=0
    for i in x:
        sum+=int(i) 
    return sum
def g(i):
    n=1
    sf_value=sf(n)
    while(n!=sf_value):
        n+=1
        sf_value=sf(n)
    return n

def sg(i):
    n=i
    x=str(n)
    sum=0
    for i in x:
        sum+=int(i)
    return sum%m
n=int(input())
for i in range(n):
    n,m=map(int,input().split())
    x=f(n)
    print(x)
    y=sf(x)
    print(y)
    z=g(y)
    print(z)
    print(sg(z))
