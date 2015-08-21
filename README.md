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
bandit1@melinda:~$ ls     
-  
bandit1@melinda:~$ ls -A   
-  .bash_logout  .bashrc  .profile  
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
ssh bandit13@bandit.labs.overthewire.org  
8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL  
ssh -i ./sshkey.private bandit14@localhost    

#Bandit 14 -> Bandit 15  
nc localhost 30000  
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e  

#Bandit 15 -> Bandit 16  
ssh bandit15@bandit.labs.overthewire.org  
BfMYroe26WYalil77FoDi9qh59eK5xNr  
echo "BfMYroe26WYalil77FoDi9qh59eK5xNr" | openssl s_client -ign_eof -connect localhost:30001  

#Bandit 16 -> Bandit 17  
ssh bandit16@bandit.labs.overthewire.org  
cluFn7wTiGryunymYOu4RcffSxQluehd  
namp -p 31000-32000 localhost  
echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -ign_eof -connect localhost:31790  

mkdir -p /tmp/strom2  
cd /tmp/strom2  
touch mmm.private  
ssh -i ./mm.private bandit17@localhost  

#Bandit 17 -> Bandit 18
ls  
diff passwords.new passwords.old  

#Bandit 18 -> Bandit 19  
ssh -T bandit18@bandit.labs.overthewire.org  
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd    
ls 
cat readme   

#Bandit 19 -> Bandit 20  
ssh bandit19@bandit.labs.overthewire.org
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x  
ls  
ls -l  
./bandit20-do cat /etc/bandit_pass/bandit20  

#Bandit 20 -> Bandit 21  
ssh bandit20@bandit.labs.overthewire.org  
GbKksEFF4yrVs6il55v6gwY5aVje5f0j    






