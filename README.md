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





