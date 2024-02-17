## vulnserver

> damiano gubiani

using the function TRUN of vulnserver to get 
a reverse shell by exploiting the buffer overflow

# step: 1
---------

with the program spike i started to fuzz the parameter trun
i wrote a little script to do that

'''bash
s_readline()
s_string("TRUN ")
s_string_variable("FUZZ")
'''



