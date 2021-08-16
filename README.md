n = input()
t = 0 
p= 0
ch = 0
sp = 0
sem = 1
nol = 0
for i in n:
    if i == "3":
        t=t+1
    if i == n[-1]:
        p =p +1
    if int(i) % 2 == 0:
        ch =ch + 1
    if int(i)>5:
        sp = sp + int(i)
    if int(i) > 7:
        sem = sem * int(i)
    if int(i) == 0 or int(i) == 5:
        nol = nol + 1
        
print(t, p, ch, sp, sem,nol, sep="\n")
