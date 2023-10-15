# logon

No matter what credentials we use for the login, it successfully logs us in but doesn't give us the flag. This suggests that a cookie might be used to store a separate variable that might be preventing us from seeing the flag. Sure enough, we notice an admin cookie set to False. Changing this to True and refreshing the page gives us the flag:picoCTF{th3_c0nsp1r4cy_l1v3s_0c98aacc}

