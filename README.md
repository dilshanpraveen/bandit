**IT13007652**
#Bandit 0 -> Bandit 1  
root@bt:~# ssh bandit0@bandit.labs.overthewire.org  
bandit0@bandit.labs.overthewire.org's password:bandit0  
bandit0@melinda:~$ ls        
readme  
bandit0@melinda:~$ cat readme   
boJ9jbbUNNfktd78OOpsqOltutMc3MY1  
bandit0@melinda:~$     

#Bandit 1 -> Bandit 2    
root@bt:~# ssh bandit1@bandit.labs.overthewire.org      
bandit1@bandit.labs.overthewire.org's password:boJ9jbbUNNfktd78OOpsqOltutMc3MY1  
bandit1@melinda:~$             
bandit1@melinda:~$ ls       
\-   
bandit1@melinda:~$ ls -A               
\-  .bash_logout  .bashrc  .profile              
bandit1@melinda:~$ cat ./-                    
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9               
bandit1@melinda:~$              
       

#Bandit 2 -> Bandit 3  
root@bt:~# ssh bandit2@bandit.labs.overthewire.org  
bandit2@bandit.labs.overthewire.org's password:CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9    
bandit2@melinda:~$ ls  
spaces in this filename  
bandit2@melinda:~$ cat spaces\ in\ this\ filename   
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK    
bandit2@melinda:~$     

#Bandit 3 -> Bandit 4  
root@bt:~# ssh bandit3@bandit.labs.overthewire.org  
bandit3@bandit.labs.overthewire.org's password:UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK      
bandit3@melinda:~$ ls  
inhere  
bandit3@melinda:~$ cd inhere/   
bandit3@melinda:~/inhere$ ls    
bandit3@melinda:~/inhere$ ls -A   
.hidden   
bandit3@melinda:~/inhere$ cat .hidden    
pIwrPrtPN36QITSp3EQaw936yaFoFgAB   
bandit3@melinda:~/inhere$    
  
#Bandit 4 -> Bandit 5
root@bt:~# ssh bandit4@bandit.labs.overthewire.org    
bandit4@bandit.labs.overthewire.org's password:pIwrPrtPN36QITSp3EQaw936yaFoFgAB    
bandit4@melinda:~$ ls  
inhere  
bandit4@melinda:~$ cd inhere/  
bandit4@melinda:~/inhere$ ls  
-file00  -file02  -file04  -file06  -file08   
-file01  -file03  -file05  -file07  -file09   
bandit4@melinda:~/inhere$ cat ./-file00   
;�-i�(��z��У��ޘ�鑾bandit4@melinda:~/inhere$ cat ./-file01
?�@c   
    O8�L��c�Ч7�zb~��ף���Ubandit4@melinda:~/inhere$ cat ./-file02
�g�f�4�6+>"��B�Vx��d��;de�Obandit4@melinda:~/inhere$ cat ./-file03
�:n����8S��Ѕ[�/q�(��@��M�.�tbandit4@melinda:~/inhere$ cat ./-file04
����+��5�`�R
�1*6C�u#Nr�bandit4@melinda:~/inhere$ cat ./-file05
��hZ����P�邚���{#��TP��6�]��X:bandit4@melinda:~/inhere$ cat ./-file06
����!��>P�
d{��ҏH�xX|�bandit4@melinda:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh   
bandit4@melinda:~/inhere$    
  
#Bandit 5 -> Bandit 6  
root@bt:~# ssh bandit5@bandit.labs.overthewire.org    
bandit5@bandit.labs.overthewire.org's password:koReBOKuIDDepwhWk7jZC0RTdopnAYKh   
bandit5@melinda:~$ ls  
inhere  
bandit5@melinda:~$ cd inhere/  
bandit5@melinda:~/inhere$ ls  
maybehere00  maybehere04  maybehere08  maybehere12  maybehere16  
maybehere01  maybehere05  maybehere09  maybehere13  maybehere17  
maybehere02  maybehere06  maybehere10  maybehere14  maybehere18  
maybehere03  maybehere07  maybehere11  maybehere15  maybehere19  
bandit5@melinda:~/inhere$ find -type f -size 1033c  
./maybehere07/.file2  
bandit5@melinda:~/inhere$ cat ./maybehere07/.file2  
DXjZPULLxYr17uwoI01bNLQbtFemEgo7  
bandit5@melinda:~/inhere$   

#Bandit 6 -> Bandit 7    
root@bt:~# ssh bandit6@bandit.labs.overthewire.org   
bandit6@bandit.labs.overthewire.org's password:DXjZPULLxYr17uwoI01bNLQbtFemEgo7  
bandit6@melinda:~$     
bandit6@melinda:~$ ls    
bandit6@melinda:~$ ls -A    
.bash_logout  .bashrc  .profile    
bandit6@melinda:~$ find / -user bandit7 -group bandit6 -size 33c    
ind: `/root': Permission denied  
find: `/proc/tty/driver': Permission denied  
find: `/proc/20130/task/20130/fd/5': No such file or directory  
find: `/proc/20130/task/20130/fdinfo/5': No such file or directory   
find: `/proc/20130/fd/5': No such file or directory  
find: `/proc/20130/fdinfo/5': No such file or directory  
find: `/etc/krypton_pass': Permission denied  
find: `/etc/chatscripts': Permission denied  
find: `/etc/natas_session_toucher': Permission denied  
find: `/etc/ssl/private': Permission denied  
find: `/etc/natas_pass': Permission denied    
find: `/etc/ppp/peers': Permission denied    
find: `/run/user/12006': Permission denied      
find: `/run/user/11019': Permission denied          
find: `/run/user/11010': Permission denied          
find: `/run/user/11011': Permission denied           
find: `/run/user/11002': Permission denied       
find: `/run/user/11009': Permission denied        
find: `/run/user/11000': Permission denied       
find: `/run/user/11001': Permission denied        
find: `/run/user/12000': Permission denied          
find: `/run/user/11013': Permission denied      
find: `/run/user/13000': Permission denied            
find: `/run/user/12002': Permission denied         
find: `/run/user/14008': Permission denied        
find: `/run/user/11005': Permission denied             
find: `/run/user/15002': Permission denied                 
find: `/run/user/14002': Permission denied                  
find: `/run/user/11012': Permission denied                    
find: `/run/user/11022': Permission denied                   
find: `/run/user/11014': Permission denied                 
find: `/run/user/11024': Permission denied              
find: `/run/user/11004': Permission denied             
find: `/run/user/14006': Permission denied               
find: `/run/user/12003': Permission denied               
find: `/run/user/12005': Permission denied             
find: `/run/user/11015': Permission denied           
find: `/run/user/11016': Permission denied            
find: `/run/user/5003': Permission denied         
find: `/run/user/13003': Permission denied         
find: `/run/user/14001': Permission denied            
find: `/run/user/5016': Permission denied            
find: `/run/user/12001': Permission denied             
find: `/run/user/11023': Permission denied                  
find: `/run/user/11018': Permission denied 
find: `/run/user/17004': Permission denied         
find: `/run/user/8005': Permission denied        
find: `/run/user/8004': Permission denied     
find: `/run/user/8002': Permission denied         
find: `/run/user/8001': Permission denied          
find: `/run/user/6004': Permission denied      
find: `/run/user/0': Permission denied          
find: `/run/user/11020': Permission denied           
find: `/run/user/14007': Permission denied              
find: `/run/shm': Permission denied            
find: `/tmp': Permission denied              
find: `/lost+found': Permission denied               
find: `/var/lib/sudo': Permission denied            
find: `/var/lib/php5': Permission denied            
find: `/var/lib/cron-apt/_-_etc_-_cron-apt_-_config': Permission denied         
find: `/var/lib/mysql': Permission denied           
/var/lib/dpkg/info/bandit7.password           
find: `/var/cache/ldconfig': Permission denied          
find: `/var/log': Permission denied             
find: `/var/lock': Permission denied                
find: `/var/crash': Permission denied               
find: `/var/spool/cron/atspool': Permission denied            
find: `/var/spool/cron/crontabs': Permission denied            
find: `/var/spool/cron/atjobs': Permission denied            
find: `/var/spool/rsyslog': Permission denied            
find: `/var/tmp': Permission denied         
find: `/var/www/melinda/stats': Permission denied                
find: `/var/www/natas/natas11': Permission denied          
find: `/var/www/natas/natas25': Permission denied               
find: `/var/www/natas/natas9': Permission denied               
find: `/var/www/natas/natas22': Permission denied               
find: `/var/www/natas/natas17': Permission denied                 
find: `/var/www/natas/natas3': Permission denied               
find: `/var/www/natas/natas20': Permission denied                  
find: `/var/www/natas/natas14': Permission denied               
find: `/var/www/natas/natas19': Permission denied                      
find: `/var/www/natas/natas21-experimenter': Permission denied              
find: `/var/www/natas/natas21': Permission denied                    
find: `/var/www/natas/natas28': Permission denied             
find: `/var/www/natas/natas6': Permission denied             
find: `/var/www/natas/natas7': Permission denied                
find: `/var/www/natas/natas10': Permission denied             
find: `/var/www/natas/natas13': Permission denied               
find: `/var/www/natas/natas26': Permission denied            
find: `/var/www/natas/stats': Permission denied               
find: `/var/www/natas/natas24': Permission denied            
find: `/var/www/natas/natas0': Permission denied          
find: `/var/www/natas/natas15': Permission denied             
find: `/var/www/natas/natas8': Permission denied             
find: `/var/www/natas/natas12': Permission denied            
find: `/var/www/natas/natas27': Permission denied             
find: `/var/www/natas/natas18': Permission denied            
find: `/var/www/natas/natas16': Permission denied             
find: `/var/www/natas/natas2': Permission denied                
find: `/var/www/natas/natas5': Permission denied          
find: `/var/www/natas/natas4': Permission denied               
find: `/var/www/natas/natas23': Permission denied           
find: `/var/www/natas/natas1': Permission denied          
find: `/drifter/drifter14_src/axTLS': Permission denied             
find: `/home/bandit5/inhere': Permission denied            
find: `/home/leviathan0/.backup': Permission denied            
find: `/home/drifter6/data': Permission denied              
find: `/home/leviathan4/.trash': Permission denied             
find: `/home/drifter8/chroot': Permission denied           
find: `/sys/kernel/debug': Permission denied             
bandit6@melinda:~$       
bandit6@melinda:~$ cd /var/lib/dpkg/info      
bandit6@melinda:/var/lib/dpkg/info$ cat bandit7.password   
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs    
bandit6@melinda:/var/lib/dpkg/info$         
   
#Bandit 7 -> Bandit 8    
root@bt:~# ssh bandit7@bandit.labs.overthewire.org   
bandit7@bandit.labs.overthewire.org's password:HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs    
bandit7@melinda:~$ ls  
data.txt  
bandit7@melinda:~$ grep 'millionth' data.txt  
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV  
bandit7@melinda:~$    

#Bandit 8 -> Bandit 9  
root@bt:~# ssh bandit8@bandit.labs.overthewire.org  
bandit8@bandit.labs.overthewire.org's password:cvX2JJa4CFALtqS87jk27qwqGhBM9plV    
bandit8@melinda:~$ ls  
data.txt  
bandit8@melinda:~$ cat data.txt | sort | uniq -u  
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR  
bandit8@melinda:~$     

#Bandit 9 -> Bandit 10   
root@bt:~# ssh bandit9@bandit.labs.overthewire.org    
bandit9@bandit.labs.overthewire.org's password:UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR    
bandit9@melinda:~$ ls                                 
data.txt  
bandit9@melinda:~$ string data.txt | grep '=' | sort  
-bash: string: command not found  
bandit9@melinda:~$ strings data.txt | grep '=' | sort  
/(Ne=  
7?YD=  
========== ism  
========== password  
========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk  
?M=HqAH  
C=_"  
I========== the6  
N$=&  
`h(8=`  
epr~F=K   
f=C(  
ie)=5e  
l/a=L)  
n\H=;  
z5Y=  
bandit9@melinda:~$    

#Bandit 10 -> Bandit 11
root@bt:~# ssh bandit10@bandit.labs.overthewire.org  
bandit10@bandit.labs.overthewire.org's password:truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk     
bandit10@melinda:~$ ls  
data.txt  
bandit10@melinda:~$ file data.txt   
data.txt: ASCII text    
bandit10@melinda:~$ base64 -d data.txt   
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR  
bandit10@melinda:~$     

#Bandit 11 -> Bandit 12  
root@bt:~# ssh bandit11@bandit.labs.overthewire.org   
bandit11@bandit.labs.overthewire.org's password:IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR     
bandit11@melinda:~$ ls   
data.txt  
bandit11@melinda:~$ file data.txt   
data.txt: ASCII text  
bandit11@melinda:~$ cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'   
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu 
bandit11@melinda:~$      

#Bandit 12 -> Bandit 13   
root@bt:~# ssh bandit12@bandit.labs.overthewire.org  
bandit12@bandit.labs.overthewire.org's password:5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu  
bandit12@melinda:~$ ls     
data.txt          
bandit12@melinda:~$ file data.txt     
data.txt: ASCII text                
bandit12@melinda:~$ cd /temp                 
-bash: cd: /temp: No such file or directory                  
bandit12@melinda:~$ cd /tmp                 
bandit12@melinda:/tmp$ mkdir mule1              
bandit12@melinda:/tmp$ cd mule1            
bandit12@melinda:/tmp/mule1$           
bandit12@melinda:/tmp/mule1$ cp ~/data.txt /tmp/mule1          
bandit12@melinda:/tmp/mule1$ xxd-r data.txt 5        
-bash: xxd-r: command not found             
bandit12@melinda:/tmp/mule1$ xxd -r data.txt 5         
bandit12@melinda:/tmp/mule1$ file 5        
5: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression     
bandit12@melinda:/tmp/mule1$ mv 5 5.gz       
bandit12@melinda:/tmp/mule1$ gzip -d 5.gz         
bandit12@melinda:/tmp/mule1$ ls            
5  data.txt           
bandit12@melinda:/tmp/mule1$ file 5            
5: bzip2 compressed data, block size = 900k             
bandit12@melinda:/tmp/mule1$ mv 5 5.bz2               
bandit12@melinda:/tmp/mule1$ bzip2 -d 5.bz2                
bandit12@melinda:/tmp/mule1$ ls               
5  data.txt               
bandit12@melinda:/tmp/mule1$ file 5              
5: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression       
bandit12@melinda:/tmp/mule1$ mv 5 5.gz            
bandit12@melinda:/tmp/mule1$ gzip -d 5.gz             
bandit12@melinda:/tmp/mule1$ ls           
5  data.txt                     
bandit12@melinda:/tmp/mule1$ file 5             
5: POSIX tar archive (GNU)                 
bandit12@melinda:/tmp/mule1$ mv 5 5.tar                     
bandit12@melinda:/tmp/mule1$ tar -xvf 5.tar             
data5.bin                     
bandit12@melinda:/tmp/mule1$ file data5.bin                
data5.bin: POSIX tar archive (GNU)                           
bandit12@melinda:/tmp/mule1$ tar -xvf data5.bin                 
data6.bin                              
bandit12@melinda:/tmp/mule1$ mv data6.bin data6.bz2                       
bandit12@melinda:/tmp/mule1$ bzip2 -d data6.bz2                         
bandit12@melinda:/tmp/mule1$ ls                            
5.tar  data.txt  data5.bin  data6                    
bandit12@melinda:/tmp/mule1$ file data6                  
data6: POSIX tar archive (GNU)                    
bandit12@melinda:/tmp/mule1$ tar -xvf data6                 
data8.bin                 
bandit12@melinda:/tmp/mule1$ file data8.bin        
data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression    
bandit12@melinda:/tmp/mule1$ mv data8.bin data8.bin.gz       
bandit12@melinda:/tmp/mule1$ gzip -d data8.bin.gz                    
bandit12@melinda:/tmp/mule1$ ls                    
5.tar  data.txt  data5.bin  data6  data8.bin                  
bandit12@melinda:/tmp/mule1$ file data8.bin                     
data8.bin: ASCII text                             
bandit12@melinda:/tmp/mule1$ cat data8.bin                   
The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL                     
bandit12@melinda:/tmp/mule1$                                 

#Bandit 13 -> Bandit 14
 root@bt:~# ssh bandit13@bandit.labs.overthewire.org    
bandit13@bandit.labs.overthewire.org's password:8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL    
bandit13@melinda:~$              
bandit13@melinda:~$ ssh -i ./sshkey.private bandit14@localhost              
Could not create directory '/home/bandit13/.ssh'.                      
The authenticity of host 'localhost (127.0.0.1)' can't be established.            
ECDSA key fingerprint is 05:3a:1c:25:35:0a:ed:2f:cd:87:1c:f6:fe:69:e4:f6.                 
Are you sure you want to continue connecting (yes/no)? yes       
bandit14@melinda:~$                 
bandit14@melinda:~$ cat /etc/bandit_pass/bandit14           
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e           
bandit14@melinda:~$                


#Bandit 14 -> Bandit 15  
bandit14@melinda:~$                 
bandit14@melinda:~$ nc localhost 30000                   
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e                  
Correct!          
BfMYroe26WYalil77FoDi9qh59eK5xNr          
               
bandit14@melinda:~$                  

#Bandit 15 -> Bandit 16  
root@bt:~# ssh bandit15@bandit.labs.overthewire.org    
bandit15@bandit.labs.overthewire.org's password:BfMYroe26WYalil77FoDi9qh59eK5xNr            
bandit15@melinda:~$ echo "BfMYroe26WYalil77FoDi9qh59eK5xNr" | openssl s_client -ign_eof -connect localhost:30001        
CONNECTED(00000003)                                      
depth=0 CN = li190-250.members.linode.com                  
verify error:num=18:self signed certificate                   
verify return:1                   
depth=0 CN = li190-250.members.linode.com                  
verify return:1                              
\---    
Certificate chain    
 0 s:/CN=li190-250.members.linode.com   
   i:/CN=li190-250.members.linode.com    
\---   
Server certificate    
\-----BEGIN CERTIFICATE-----    
MIIC3jCCAcagAwIBAgIJAI5QiWZw4YHbMA0GCSqGSIb3DQEBCwUAMCcxJTAjBgNV
BAMTHGxpMTkwLTI1MC5tZW1iZXJzLmxpbm9kZS5jb20wHhcNMTQxMTE0MTAyODA0
WhcNMjQxMTExMTAyODA0WjAnMSUwIwYDVQQDExxsaTE5MC0yNTAubWVtYmVycy5s
aW5vZGUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsKmy9o5z
WU+1EH7Z3bB5TGQA+16zXDcEJy6tZWZ8CDrRyQXiahendp45BWUc/ZuLDo0+B3Wt
ZXjofmLw/F4fmR+8X1s1fQZX2dFt920qEm7LxqzWd0c7FdHiBwwRrwhkk+3cQpOB
TTGdLWEgpdmwwNZDTUdsDLzjDczPnju6T6p6ArTECztPbmTjfY4QIRtC6capL1Z+
yPJSQVAuAMEX1wTDWTGdm0VV7oW4F5cGZutf6QAP51jdhSyZuGilIPHbnj0l6Qc7
a7+OtEsEGi31aJ8KpRf7LNZ7DXCuoB3Hf75Pd6VjDgoOIagcH0NYqa75gEjBkGzs
ktLWykT7ag7fKwIDAQABow0wCzAJBgNVHRMEAjAAMA0GCSqGSIb3DQEBCwUAA4IB
AQCaZdUNAj8WDEKWdoU3LNXUBJlTJwiWBrh550PbHSQORcCz2K0kiMei1A4ojK2N
dMHFGAqAeUEaxtz92p2BoFpZasAtdSa3u63tBckFhfUolIS1TC7Cj51y19ysTeep
fGPFpuPCVqVPsruei8Z/iqn3bFIhQQdmumeePZQdPMwZSWHNVYC5XODd7PvNDrDu
5MZJjkz4+6LbwwAvyew62meFN2QEsYbK2Brtbhze+IjE27FGWlSw4K3jlwa409MD
MTf4JU41ELaYY8G/LSNDJsBVhhkHzvXR9iCbXxNz3IL0dQDNj7h4LKhBy0q7hvqg
kDzwlmBO4WKSmCAuky44cXmd  
\-----END CERTIFICATE-----   
subject=/CN=li190-250.members.linode.com  
issuer=/CN=li190-250.members.linode.com  
\---   
No client certificate CA names sent  
\---  
SSL handshake has read 1714 bytes and written 637 bytes     
\---  
New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA  
Server public key is 2048 bit   
Secure Renegotiation IS supported     
Compression: NONE              
Expansion: NONE                   
SSL-Session:                  
    Protocol  : SSLv3                   
    Cipher    : DHE-RSA-AES256-SHA                         
    Session-ID: 465F582880BA3493B95D60AFD027F193E8D7C10B87FE56346266255B05700E0A        
    Session-ID-ctx:                  
    Master-Key: B3B221F6334CEC2045D364AEC7D0B8DD8F021316AEE9F9D51B0E1B9E9A1DEA59864FD6309DC0CFD65E2BD8EB22FF01B5      
    Key-Arg   : None  
    PSK identity: None                    
    PSK identity hint: None               
    SRP username: None   
    Start Time: 1440147446     
    Timeout   : 300 (sec)     
    Verify return code: 18 (self signed certificate)   
\--- 
Correct!               
cluFn7wTiGryunymYOu4RcffSxQluehd              
       
read:errno=0          
bandit15@melinda:~$                      

#Bandit 16 -> Bandit 17  
root@bt:~# ssh bandit16@bandit.labs.overthewire.org      
bandit16@bandit.labs.overthewire.org's password:cluFn7wTiGryunymYOu4RcffSxQluehd       
bandit16@melinda:~$               
bandit16@melinda:~$ nmap -p 31000-32000 localhost                 

Starting Nmap 6.40 ( http://nmap.org ) at 2015-08-21 09:09 UTC            
Nmap scan report for localhost (127.0.0.1)          
Host is up (0.00085s latency).                   
Not shown: 996 closed ports                    
PORT      STATE SERVICE                     
31046/tcp open  unknown                    
31518/tcp open  unknown                   
31691/tcp open  unknown                 
31790/tcp open  unknown                 
31960/tcp open  unknown           
 
Nmap done: 1 IP address (1 host up) scanned in 0.07 seconds                       
bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -ign_eof -connect localhost:31046        
CONNECTED(00000003)                         
140737354045088:error:140770FC:SSL routines:SSL23_GET_SERVER_HELLO:unknown protocol:s23_clnt.c:795:     
\---         
no peer certificate available                     
\---   
No client certificate CA names sent   
\---      
SSL handshake has read 7 bytes and written 295 bytes        
\--      
New, (NONE), Cipher is (NONE)     
Secure Renegotiation IS NOT supported                   
Compression: NONE                    
Expansion: NONE              
\---              
bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -ign_eof -connect localhost:31518  
CONNECTED(00000003)    
depth=0 CN = li190-250.members.linode.com       
verify error:num=18:self signed certificate                    
verify return:1                  
depth=0 CN = li190-250.members.linode.com                   
verify return:1       
\---      
Certificate chain     
 0 s:/CN=li190-250.members.linode.com                    
   i:/CN=li190-250.members.linode.com          
\---              
Server certificate                
\-----BEGIN CERTIFICATE-----            
MIIC3jCCAcagAwIBAgIJAI5QiWZw4YHbMA0GCSqGSIb3DQEBCwUAMCcxJTAjBgNV
BAMTHGxpMTkwLTI1MC5tZW1iZXJzLmxpbm9kZS5jb20wHhcNMTQxMTE0MTAyODA0
WhcNMjQxMTExMTAyODA0WjAnMSUwIwYDVQQDExxsaTE5MC0yNTAubWVtYmVycy5s
aW5vZGUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsKmy9o5z
WU+1EH7Z3bB5TGQA+16zXDcEJy6tZWZ8CDrRyQXiahendp45BWUc/ZuLDo0+B3Wt
ZXjofmLw/F4fmR+8X1s1fQZX2dFt920qEm7LxqzWd0c7FdHiBwwRrwhkk+3cQpOB
TTGdLWEgpdmwwNZDTUdsDLzjDczPnju6T6p6ArTECztPbmTjfY4QIRtC6capL1Z+
yPJSQVAuAMEX1wTDWTGdm0VV7oW4F5cGZutf6QAP51jdhSyZuGilIPHbnj0l6Qc7
a7+OtEsEGi31aJ8KpRf7LNZ7DXCuoB3Hf75Pd6VjDgoOIagcH0NYqa75gEjBkGzs
ktLWykT7ag7fKwIDAQABow0wCzAJBgNVHRMEAjAAMA0GCSqGSIb3DQEBCwUAA4IB
AQCaZdUNAj8WDEKWdoU3LNXUBJlTJwiWBrh550PbHSQORcCz2K0kiMei1A4ojK2N
dMHFGAqAeUEaxtz92p2BoFpZasAtdSa3u63tBckFhfUolIS1TC7Cj51y19ysTeep
fGPFpuPCVqVPsruei8Z/iqn3bFIhQQdmumeePZQdPMwZSWHNVYC5XODd7PvNDrDu
5MZJjkz4+6LbwwAvyew62meFN2QEsYbK2Brtbhze+IjE27FGWlSw4K3jlwa409MD
MTf4JU41ELaYY8G/LSNDJsBVhhkHzvXR9iCbXxNz3IL0dQDNj7h4LKhBy0q7hvqg
kDzwlmBO4WKSmCAuky44cXmd             
\-----END CERTIFICATE-----             
subject=/CN=li190-250.members.linode.com                 
issuer=/CN=li190-250.members.linode.com                
 ---              
No client certificate CA names sent            
\---           
SSL handshake has read 1714 bytes and written 637 bytes               
\---              
New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA                
Server public key is 2048 bit           
Secure Renegotiation IS supported                   
Compression: NONE            
Expansion: NONE                 
SSL-Session:          
    Protocol  : SSLv3                           
    Cipher    : DHE-RSA-AES256-SHA                              
    Session-ID: 82EE7A5EED336E724CE2D42EA5AE2B3683EEE297FCD9884C49900DC703304B79               
    Session-ID-ctx:            
    Master-Key: 89CC03D96B81BC1F258E0DD8E319AEA50C9C7548368E9B9B4BFCA86660C9A5D605A8E9609E759754612ECC95C741AB7F       
    Key-Arg   : None           
    PSK identity: None              
    PSK identity hint: None                
    SRP username: None               
    Start Time: 1440148223                
    Timeout   : 300 (sec)                 
    Verify return code: 18 (self signed certificate)          
\---   
cluFn7wTiGryunymYOu4RcffSxQluehd                 
^C                    
bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -ign_eof -connect localhost:31691     
CONNECTED(00000003)   
140737354045088:error:140770FC:SSL routines:SSL23_GET_SERVER_HELLO:unknown protocol:s23_clnt.c:795:     
\---             
no peer certificate available               
\---                 
No client certificate CA names sent                
\---
SSL handshake has read 7 bytes and written 295 bytes                 
\---                      
New, (NONE), Cipher is (NONE)                               
Secure Renegotiation IS NOT supported
Compression: NONE                                       
Expansion: NONE                 
\---                                           
bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -ign_eof -connect localhost:31790     
CONNECTED(00000003)    
depth=0 CN = li190-250.members.linode.com                   
verify error:num=18:self signed certificate              
verify return:1                
depth=0 CN = li190-250.members.linode.com                 
verify return:1           
\---                         
Certificate chain       
 0 s:/CN=li190-250.members.linode.com               
   i:/CN=li190-250.members.linode.com                     
\---                       
Server certificate                    
\-----BEGIN CERTIFICATE-----     
MIIC3jCCAcagAwIBAgIJAI5QiWZw4YHbMA0GCSqGSIb3DQEBCwUAMCcxJTAjBgNV
BAMTHGxpMTkwLTI1MC5tZW1iZXJzLmxpbm9kZS5jb20wHhcNMTQxMTE0MTAyODA0
WhcNMjQxMTExMTAyODA0WjAnMSUwIwYDVQQDExxsaTE5MC0yNTAubWVtYmVycy5s
aW5vZGUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsKmy9o5z
WU+1EH7Z3bB5TGQA+16zXDcEJy6tZWZ8CDrRyQXiahendp45BWUc/ZuLDo0+B3Wt
ZXjofmLw/F4fmR+8X1s1fQZX2dFt920qEm7LxqzWd0c7FdHiBwwRrwhkk+3cQpOB
TTGdLWEgpdmwwNZDTUdsDLzjDczPnju6T6p6ArTECztPbmTjfY4QIRtC6capL1Z+
yPJSQVAuAMEX1wTDWTGdm0VV7oW4F5cGZutf6QAP51jdhSyZuGilIPHbnj0l6Qc7
a7+OtEsEGi31aJ8KpRf7LNZ7DXCuoB3Hf75Pd6VjDgoOIagcH0NYqa75gEjBkGzs
ktLWykT7ag7fKwIDAQABow0wCzAJBgNVHRMEAjAAMA0GCSqGSIb3DQEBCwUAA4IB
AQCaZdUNAj8WDEKWdoU3LNXUBJlTJwiWBrh550PbHSQORcCz2K0kiMei1A4ojK2N
dMHFGAqAeUEaxtz92p2BoFpZasAtdSa3u63tBckFhfUolIS1TC7Cj51y19ysTeep
fGPFpuPCVqVPsruei8Z/iqn3bFIhQQdmumeePZQdPMwZSWHNVYC5XODd7PvNDrDu
5MZJjkz4+6LbwwAvyew62meFN2QEsYbK2Brtbhze+IjE27FGWlSw4K3jlwa409MD
MTf4JU41ELaYY8G/LSNDJsBVhhkHzvXR9iCbXxNz3IL0dQDNj7h4LKhBy0q7hvqg
kDzwlmBO4WKSmCAuky44cXmd           
\-----END CERTIFICATE-----                   
subject=/CN=li190-250.members.linode.com                   
issuer=/CN=li190-250.members.linode.com             
\---                       
No client certificate CA names sent                
\---                                               
SSL handshake has read 1714 bytes and written 637 bytes                      
\ ---                         
New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA                 
Server public key is 2048 bit             
Secure Renegotiation IS supported               
Compression: NONE               
Expansion: NONE              
SSL-Session:               
    Protocol  : SSLv3               
    Cipher    : DHE-RSA-AES256-SHA                              
    Session-ID: C8C6CFB8EB9F4F6C0D05D59D4A38029EEE4C034775D0A58C7305C0EBCCAA7340                
    Session-ID-ctx:                          
    Master-Key: EEB44FD8C43CC2C3426E435F2649D1C470F0EAC3BB6B07A3104DCAB29EDE83398937C662D01D22CD8BB55E51A27AEBAE          
    Key-Arg   : None                                  
    PSK identity: None           
    PSK identity hint: None                
    SRP username: None              
    Start Time: 1440148243             
    Timeout   : 300 (sec)               
    Verify return code: 18 (self signed certificate)                   
\---             
Correct!                          
\----BEGIN RSA PRIVATE KEY-----    
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=   
\-----END RSA PRIVATE KEY-----   
   
read:errno=0        
bandit16@melinda:~$                                   
bandit16@melinda:~$ mkdir -p /tmp/mule2                     
bandit16@melinda:~$ cd /tmp/mule2                    
bandit16@melinda:/tmp/key$ touch uu.private                         
bandit16@melinda:/tmp/key$ vim uu.private                       
bandit16@melinda:/tmp/key$ ssh -i ./uu.private bandit17@localhost                      
Could not create directory '/home/bandit16/.ssh'.                     
The authenticity of host 'localhost (127.0.0.1)' can't be established.                 
ECDSA key fingerprint is 05:3a:1c:25:35:0a:ed:2f:cd:87:1c:f6:fe:69:e4:f6.
Are you sure you want to continue connecting (yes/no)? yes                                  

#Bandit 17 -> Bandit 18                          
bandit17@melinda:~$ ls
passwords.new  passwords.old
bandit17@melinda:~$ diff passwords.new passwords.old
42c42
\< kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
\---
\> BS8bqB1kqkinKJjuxL6k072Qq9NRwQpR
bandit17@melinda:~$   
  
#Bandit 18 -> Bandit 19    
root@bt:~# ssh bandit18@bandit.labs.overthewire.org  
bandit18@bandit.labs.overthewire.org's password:kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd   
Byebye !               
Connection to bandit.labs.overthewire.org closed.                
root@bt:~#             
root@bt:~# ssh -T bandit18@bandit.labs.overthewire.org 
bandit18@bandit.labs.overthewire.org's password:kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd      
ls 
readme
cat readme   
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x   

#Bandit 19 -> Bandit 20  
root@bt:~# ssh bandit19@bandit.labs.overthewire.org  
bandit19@bandit.labs.overthewire.org's password:IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x    
bandit19@melinda:~$ ls
bandit20-do
bandit19@melinda:~$ ls -l
total 8
-rwsr-x--- 1 bandit20 bandit19 7370 Nov 14  2014 bandit20-do
bandit19@melinda:~$ ./bandit20-do
Run a command as another user.
  Example: ./bandit20-do id
bandit19@melinda:~$ ./bandit20-do id
uid=11019(bandit19) gid=11019(bandit19) euid=11020(bandit20) groups=11020(bandit20),11019(bandit19)
bandit19@melinda:~$ ./bandit20-do whoami
bandit20
bandit19@melinda:~$ ./bandit20-do cat /etc/bandit_pass/bandit20 
GbKksEFF4yrVs6il55v6gwY5aVje5f0j
bandit19@melinda:~$    

#Bandit 20 -> Bandit 21  
root@bt:~# ssh bandit20@bandit.labs.overthewire.org  
bandit20@bandit.labs.overthewire.org's password:GbKksEFF4yrVs6il55v6gwY5aVje5f0j      
bandit20@melinda:~$ 
bandit20@melinda:~$ ls
suconnect
bandit20@melinda:~$ ./suconnect 
Usage: ./suconnect <portnumber>
This program will connect to the given port on localhost using TCP. If it receives the correct password from the other side, the next password is transmitted back.
bandit20@melinda:~$ nc -l 32005
GbKksEFF4yrVs6il55v6gwY5aVje5f0j
gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
bandit20@melinda:~$   

bandit20@melinda:~$ ls
suconnect
bandit20@melinda:~$ ./suconnect 32005
Read: GbKksEFF4yrVs6il55v6gwY5aVje5f0j
Password matches, sending next password
bandit20@melinda:~$  







