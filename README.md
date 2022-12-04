# checkid
import time
from id_validator import validator
#def drange():
def vali(id1,id2):
    count = 0
    for i in range(99,10000):
        if i<1000:
            tid3=str(0)+str(i)
            tid = id1 + id2 + tid3
            if validator.is_valid(tid):
                count = count + 1
                # print(validator.get_info(tid))
                print(tid)
        else :
            tid3=str(i)
            tid=id1+id2+tid3
            if validator.is_valid(tid):
                count=count+1
                #print(validator.get_info(tid))
                print(tid)
       # print(count)
vali('','')
