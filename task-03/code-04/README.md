## RICH TONY POOR SPIDEY
#### Code


n=int(input())
for i in range(0,n):
    x=input()
    y=input()
    x=x.split()
    y=y.split()
    b=int(x[0])
    c=int(x[1])
 #   h=int(y[0])
    '''for j in range(0,b):
        if int(y[j])>h:
            h=int(y[j])
        else:
            pass'''
    ans = 1
    for m in y:
        ans *= int(m)
    max_value = 0
    for k in y:
        a = ans*(int(k)-c)//(int(k))
        if(a > max_value):
            max_value = a
    print(max_value)
