## vulnserver

> damiano gubiani

using the function TRUN of vulnserver to get 
a reverse shell by exploiting the buffer overflow

# step: 1

with the program spike i started to fuzz the parameter trun
i wrote a little script to do that

- s_readline();
- s_string("TRUN ");
- s_string_variable("FUZZ");

what this 3 lines of code does is simple

- s_readline()

read the HELP message sent by server

- s_string("TRUN ")

tells spike to use this string at the start of each fuzze 

- s_string_variable("FUZZ")

with this we declare a variable that spike use for fuzzing

