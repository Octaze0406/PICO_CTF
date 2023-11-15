using cyberchef and choosing the receipe =magic and inputing the chinese text will give the flag.
Or we can use the python code.
>>> flag="灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彥ㄴㅡて㝽"
>>> l=[]
>>> for i in range(0,len(flag),2):
...     pair_of_char=flag[i:i+2]
...     unicode_code=(ord(pair_of_char[0] <<8) + ord(pair_of_char[1]
...     l.append(char(unicode_code))
  File "<stdin>", line 3
    unicode_code=(ord(pair_of_char[0] <<8) + ord(pair_of_char[1]
                                                 ^^^^^^^^^^^^^^
SyntaxError: invalid syntax. Perhaps you forgot a comma?
>>> 




flag=picoCTF{16_bits_inst34d_of_8_e141a0f7}
flag="灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彥ㄴㅡて㝽"
>>> l=[]
>>> for i in range(0,len(flag),2):
...     pair_of_char=flag[i:i+2]
...     if len(pair_of_char) ==2:
...             unicode_code=(ord(pair_of_char[0])>>8) + ord(pair_of_char[1])
...             l.append(chr(unicode_code))
...     else:
...             print("bad")
