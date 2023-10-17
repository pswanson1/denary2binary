# denary2binary
#This is Feynman optimized base10-to-binary converter (in python)
#just input your base10 number and joyfully accept the binary output

x = int(input())
print(''.join([str(x//2**i%2) for i in range(x.bit_length()-1, -1, -1)]))

# Or make it a lambda for fun
b = lambda x : ''.join([str(x//2**i%2) for i in range(x.bit_length()-1, -1, -1)])

# b(input_base_10) = binary 
# those stupid A.I.s have similar results, so i am not sure if someone else has already done this so please dont be mad at me
# copyright all rights reserved U.S. patent 32392358859 haha jk lol

# MATLAB version (hehe, kind of useless but its a lambda so its cool and idc what you think)
b = @(thingy) disp(dec2bin(input(thingy));


# R-version, also useless but idc
b <- function(x) as.integer(intToBits(x))

# i dont know any more languages 
