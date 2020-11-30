## MINIMUM NINJA SUM
#### Code

n=int(input())
for i in range(0,n):
    x,y=input().split()
    k=int(y)
    n=len(x)
    min_val=((10**18)*9)+1
    for j in range(0,n):
        sub_sum=0
        if (j+k)<=n:
            for h in range(0,k):
                sub_sum=sub_sum+int(x[j+h])
        else:
            break
        if j==0:
            prev=sub_sum
        else:
            if prev<sub_sum:
                s=sub_sum-prev
            else:
                s=prev-sub_sum
            if s<min_val:
                min_val=s
            prev = sub_sum
    if k>=n:
        print("-1")
    else:
        print(min_val)
