# SSLPinningDemo

1. Check Concetivity 
openssl s_client -connect www.objc.io:443 </dev/null

2. Double check connectivity
openssl s_client -connect www.objc.io:443 -servername  www.objc.io </dev/null

3. Create Certificate 
openssl s_client -connect www.objc.io:443 -servername  www.objc.io </dev/null | openssl x509 -outform DER > objcio.cer
