# s9x-Message-encryption
#To encrypt messages that are typed with letters only without number


#Encrypt messages with letters only by s9x
import os
os.system("clear")

message = input () 
sev = ['a','b','c','d','e','f','g','h','i','j',
'k','l','m','n','o','p','q','r','s','t','u','v',
'w','x','y','z']
sum = ""
message =message.lower()
for i in range (len(message)):
    if message [i] not in sev :
        sum+=""
        continue
    var = 0
    var = sev.index(message[i])
    var +=1
    var=-var
    #print (sev[var],end="")
    sum+=sev[var]
print (sum)
