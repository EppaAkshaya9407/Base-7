# Base-7
num = int(input("Enter a number:"))
r=num
if num==0:
    print("0")
else:
    s=""
    if num<0:
        s="-"
        num=-num
    res=""
    while num > 0:
        res=str(num%7)+res
        num//=7
    print("Base 7 of",r,":",s+res)
