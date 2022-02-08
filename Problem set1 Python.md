Neha.Patel.BDAT1004Ps#6
def pig(s):
    s=s.lower()
    li=['a','e','i','o','u']
    if s[0] in li:
        s=s[1:]+s[0]+"way"
    else:
        s=s[1:]+s[0]+"ay"
    return s
x=input("Enter string: ")
st=pig(x)
print(st)

```

    Enter string: neha
    ehanay
    

Neha.Patel.BDAT1004Ps#7
file1=open("bldcount.txt","r")
dict1={
    '10':10,
    'one':1,
    '12':12,
    'no':0,
}
for x in file1:
    y=x.split()
    y1=int(dict1[y[2]])
    for i in range(y1):
        print(y[7],end=' ')
```

    A. A. A. A. A. A. A. A. A. A. B. AB. AB. AB. AB. AB. AB. AB. AB. AB. AB. O. O. O. O. O. O. O. O. O. O. O. O. 


Neha.Patel.BDAT1004Ps#8
def curconv(s,n):
    file1=open("currencies.txt","r")
    dict1={}
    for x in file1:
        y=x.split(' ',3)
        dict1[y[0]]=y[1]
    i=float(dict1[s])
    return n*i
n1=curconv('EUR',100)
print(n1)
```

    122.96544
    


Neha.Patel.BDAT1004Ps#9
import sys
import numpy as np
try:
    print("Trying to add 6 + 'a' ")
    r = 6 + 'a'
except:
    print("Oops!", sys.exc_info()[0], "occurred.")
```

    Trying to add 6 + 'a' 
    Oops! <class 'TypeError'> occurred.
    Next entry.
    Oops! unsupported operand type(s) for +: 'int' and 'str' occurred.
    
    


Neha.Patel.BDAT1004Ps#9
import sys
import numpy as np
a = np.array((1,2,3,4,5,6,7,8,9,10))
try:
    print("Trying to find 12th elemnt of 10 size array {}".format(a[12]))
except:
    print("Oops!", sys.exc_info()[0], "occurred.")
    print()
```

    Trying to add 6 + 'a' 
    Oops! <class 'IndexError'> occurred.
    Next entry.
    Oops! index 12 is out of bounds for axis 0 with size 10 occurred.
    
    


Neha.Patel.BDAT1004Ps#9
import sys
import numpy as np
import math
try:
    x=math.sqrt(-1.0)
except:
    print("Oops!", sys.exc_info()[0], "occurred.")
    print()
```

    Oops! <class 'ValueError'> occurred.
    
    


Neha.Patel.BDAT1004Ps#9
import sys
import numpy as np
import math
try:
    print(x100)
except:
    print("Oops!", sys.exc_info()[0], "occurred.")
    print()
```

    Oops! <class 'NameError'> occurred.
    
    



Neha.Patel.BDAT1004Ps#9
import sys
import numpy as np
import math
try:
    print(x100)
except:
    print("Oops!", sys.exc_info()[0], "occurred.")
    print()
```

    Oops! <class 'NameError'> occurred.
    
    



Neha.Patel.BDAT1004Ps#9
import sys
import numpy as np
import math
try:
    file1=open("currencies100.txt","r")
except:
    print("Oops!", sys.exc_info()[0], "occurred.")
    print()
```

    Oops! <class 'FileNotFoundError'> occurred.
    
    



Neha.Patel.BDAT1004Ps#10
def frequencies(strr):
    dict1={}
    s='abcdefghijklmnopqrstuvwxyz'
    for i in s:
        dict1[i]=0;
    for i in strr:
        if i in dict1.keys():
            dict1[i]=dict1[i]+1
    print(dict1.values())
frequencies('The quick red fox got bored and went home.')
```

    dict_values([1, 1, 1, 3, 5, 1, 1, 2, 1, 0, 1, 0, 1, 2, 4, 0, 1, 2, 0, 2, 1, 0, 1, 1, 0, 0])
    
