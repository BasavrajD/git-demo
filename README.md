
![image](https://github.com/BasavrajD/git-demo/assets/112759581/ac06fb79-eb44-46a6-a6c1-b6cca3b7cb1d)


xcdqrlpkwzoufteyahnvisgjbm
ariuxnmebsgwdfloypzjkchvtq


#hashdeep

sudo apt-get install hashdeep
1.hashdeep filename 
gives o/p=> size,md5,sha256,filename
2.hashdeep filename > hash.txt
will create new file and save the o/p there
3.hashdeep -a trial_file.txt -k hash.txt
hash computed for trial_file.txt and compared with hash.txt= audit passed
4.hashdeep -c md5 evidence_file_path > new_file.txt
for genereating only md5 
md5 is same that means no tampering done to a file

#gpg
1)To install
sudo apt-get update............sudo apt-get install gnupg
2)To generate key
gpg --gen-key
3)export the public key=
gpg --export -a key_name > public.key
4)export the private key=
gpg --export-secret-key -a key_name > private.key
5)import public key
gpg --import public.key
6)import private key
gpg --allow-secret-key-import --import private.key
7)List public keys
gpg --list-keys
8)List private keys
gpg --list-secret-keys
9)to encrypt file
nano filename.txt
gpg -e -u keyname -r keyname filename.txt
10)to decrypt file
gpg -d filename.gpg
