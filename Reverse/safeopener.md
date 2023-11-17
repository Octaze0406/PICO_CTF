Even though it's a jave script, scrolling to the end of the code we can see that it check if the user input is equal to an encoding.  
which is clearly encoded in base64 and is our password.  
So to decode : echo <base64encoding> |base64 -d
