# uniqueOccurrence
l=list(map(int,input("enter numbers: ").split()))
l.sort()
print(l)
d=[]
for i in l:
    if i not in d:
        d.append(i)

occ=[]
for i in range(0,len(d)):
    count=l.count(d[i])
    occ.append(count)

for e in range(0,len(occ)-1):
    if occ[e]==occ[e+1]:
        print('False')
        break
    else:
        print('True')
