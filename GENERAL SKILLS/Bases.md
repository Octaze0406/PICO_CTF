# 
you can use the base64 command to encode and decode Base64. If you want to decode a Base64-encoded string to binary, you can use the -d.
echo [string] | base64 -d | xxd ( xxd to give the output in the terminal itself.)
echo (string) | base64 -d filename :you want to transfer the output into.
