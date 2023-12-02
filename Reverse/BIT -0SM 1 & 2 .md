##1
Simple convert the hex value being stored into the eax registry to decimal:   
Flag: 48

##2

convert the hex being stored at [rbp-0x4] whose value was moved to eax,  
flag:654874

##3

- some value is being bultiplied and stored in eax (imul): integer multiply.
- then another value is added to it.
- to get flag of 2619997

##4
.. he one hex value is compared to another and if the comparing value is less it jumps to another function where it adds 101 to the value already stored.

:mov    DWORD PTR [rbp-0x4],0x9fe1a
<+22>:    cmp    DWORD PTR [rbp-0x4],0x2710
<+29>:    jle    0x55555555514e <main+37>
<+31>:    sub    DWORD PTR [rbp-0x4],0x65
<+35>:    jmp    0x555555555152 <main+41>
<+37>:    add    DWORD PTR [rbp-0x4],0x65
