**IT13007652**
#Bandit 0 -> Bandit 1  
ssh bandit0@bandit.labs.overthewire.org    
bandit0
ls  
vi readme  

#Bandit 1 -> Bandit 2  
ssh bandit1@bandit.labs.overthewire.org    
boJ9jbbUNNfktd78OOpsqOltutMc3MY1  
ls   
ls -A  
cat ./-   

#Bandit 2 -> Bandit 3  
ssh bandit2@bandit.labs.overthewire.org  
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9  
ls  
cat spaces\ in\ this\ filename  

#Bandit 3 -> Bandit 4  
ssh bandit3@bandit.labs.overthewire.org  
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK  
ls  
cd inhere  
ls -A  
cat .hidden  

#Bandit 4 -> Bandit 5
ssh bandit4@bandit.labs.overthewire.org  
pIwrPrtPN36QITSp3EQaw936yaFoFgAB 
ls  
cd inhere  
ls  
cat ./-file00    
cat ./-file01  
cat ./-file02  
cat ./-file03  
cat ./-file04  
cat ./-file05  
cat ./-file06  
cat ./-file07   

#Bandit 5 -> Bandit 6  
ssh bandit5@bandit.labs.overthewire.org  
koReBOKuIDDepwhWk7jZC0RTdopnAYKh  
ls  
cd inhere  
ls  
find -type f -size 1033c   
cd maybehere07  
cat ./file2  

#Bandit 6 -> Bandit 7    
ssh bandit6@bandit.labs.overthewire.org  
DXjZPULLxYr17uwoI01bNLQbtFemEgo7   
find / -user bandit7 -group6 -size 33c | grep -V -F Permission  
cd /var/lib/dpkg/info  
cat bandit7.password  

#Bandit 7 -> Bandit 8    
ssh bandit7@bandit.labs.overthewire.org  
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs  
ls  
grep 'millionth' data.txt  

#Bandit 8 -> Bandit 9  
ssh bandit8@bandit.labs.overthewire.org  
cvX2JJa4CFALtqS87jk27qwqGhBM9plV  
ls  
cat data.txt | sort | uniq -u  

#Bandit 9 -> Bandit 10   
ssh bandit9@bandit.labs.overthewire.org  
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR  
strings data.txt | grep '=' | sort   

#Bandit 10 -> Bandit 11
ssh bandit10@bandit.labs.overthewire.org  
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk  
base64 -d data.txt  

#Bandit 11 -> Bandit 12  
ssh bandit11@bandit.labs.overthewire.org  
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR  
cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'  

#Bandit 12 -> Bandit 13   
ssh bandit12@bandit.labs.overthewire.org  
5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu  
ls  
file data.txt  
cd /tmp  
mkdir strom1  
cd strom1  
cp ./data.txt /tmp/storm1  
xxd -r data.txt 5
file 5
mv 5 5.gz
gzip -d 5.gz  
ls  
file 5  
mv 5 5.bz  
bzip2 -d 5.bz2  
ls  
file 5  
mv 5 5.gz  
gzip -d 5.gz    
ls  
file 5  
mv 5 5.tar  
tar -xvf 5.tar  
file data5.bin  
tar -xvf data5.bin  
file data6.bin  
mv data6.bin data6.bz2  
bzip2 -d data6.bz2
ls  
file data6  
tar -xvf data6  
ls  
file data8.bin  
mv data8.bin data8.bin.gz  
gzip -d data8.bin.gz
ls  
file data8.bin  
cat data8.bin  

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


root@bt:~# ssh bandit0@bandit.labs.overthewire.org

bandit0@bandit.labs.overthewire.org's password: 


















