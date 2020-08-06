# Mini-Smart-Calculator.-py
#At some mini calculator which calculate integer value also and string value also. 

from word2number import w2n

#program start from here

print("Smart Calculator")

cal=[]

user=input("Enter Calculation :")

cal.append(user.split())

c1=0
c2=0
c3=0

for i in range(2):
    if(type(user)==str):
        v1=w2n.word_to_num(cal[c1][c2])# Value 1st
        v2=w2n.word_to_num(cal[c1][c2+2])#2nd value
        s1=(cal[c1][c2+1])#sign of calculation
        if(s1=="+" or s1=="plus"):
            t=(v1+v2)
            break
        if(s1=="-" or s1=="minus"):
            t=(v1-v2)
            break
        if(s1=="/" or s1=="divide"):
            t=(v1/v2)
            break
        if(s1=="*" or s1=="multiply"):
            t=(v1*v2)
            break
print("Total :",t)
    
