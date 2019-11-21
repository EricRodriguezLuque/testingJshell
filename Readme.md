# Repository for testing jshell

int n = 68; n ==> 68

byte b = 127; b ==> 127

char c = 'B'; c ==> 'B'

b = n; | Error: |  incompatible types: possible lossy conversion from int to char

C = n; | Error: | cannot find symbol | symbol: variable C

### After errors fixed

int n =68; n ==> 68

byte b =127; b ==> 127

char c = 'B'; c ==> 'B'

b = (byte) n; b ==> 68

c = (char) n; c ==> 'D'