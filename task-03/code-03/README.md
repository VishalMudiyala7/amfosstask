## RYUK AND HIS DEATH NOTES
#### Code


n=int(input())
rvalues = [int(i) for i in input().split()]
avalues = [int(i) for i in input().split()]
minvalue=avalues[0]//rvalues[0]
for i in range(0,n):
    x=avalues[i]//rvalues[i]
    if x<minvalue:
        minvalue=x
    else:
        pass
print(minvalue)
