# Hashcat


Disclaimer: This is for educational purposes only.


Name: Rory Stiff



Decscription: Hashcat is a versatile hacking tool that assists brute force attacks 
by condcuting them with hash values of passwords. I will be showing md5 hashing and
sha1 hashing password techniques with hashcat and how to protect youurself from these attacks. 


Topics being covered

1. Whats Hashcat
2. whats password hashing
3. what is a hash function
4. what are md5 hashes/sha1 hashes
5. How to do a md5/sha1 sttack with hashcat
6. How to defend against hashcat
7. summary


![image](https://github.com/user-attachments/assets/15d094a0-d7c5-462a-9e5e-fbe27db551fe)




what is hashcat?


Hashcat is an advanced password recovery tool that supports various types of password hashing algorithims. It is used to crack passwords using brute-force attacks, dictionary attacks, and hybrid attacks. Hashcat is made to have the power to speed up the cracking process.





![image](https://github.com/user-attachments/assets/4322bfea-8bf2-41fb-a2d8-fa652beea6ea)




what is password hashing?



Hashing is a proccess that converts an alphanumeric string into a fixed-size string by using a hash function. This may be fimiliar as in the advanced data structure courses when they teach dictionarys we often see this when disscusing them.


what is a hash function?

Hash function: A hash function is a mathamatical function that takes in the input string and generates another alphanumeric string.


Here is what a mathamtical hash function looks like...


![image](https://github.com/user-attachments/assets/f792d945-1b31-4018-bf83-0e31dfb74d81)




Here is the mathamaitcal formula for hash functions...


Hash key % table size

Example table

![image](https://github.com/user-attachments/assets/9a496983-0f6d-4913-889c-d7340dcfaaba)


what is md5 hash/sh1 hashes?

md5 hash: md5(message digest alogrithim) is a hash function that produces a 128-bit(16-byte) hash value.

md5 hash: 42f749ade7f9e195bf475f37a44cafcb

sha1 hash: sha1(secure hash algrithim) is a hash function that produces 160-bit(20-byte) hash values.

sha1 hash: b2e98ad6f6eb8508dd6a14cfa704bad7f05f6fb1





How to do a md5/sha1 sttack with hashcat

Note: You will need to find or download a common password list


Dictionary attacks:

md5 hash 

command

$ hashcat -m 0 -a 0 md5.txt passwordlist.txt


The command above is a dictionary attack using the hashing algrithim md5. The 0 specifies the md5 hash mode. For the flag I am using -a


result of dictionary attack on md5 hash algrithim



![image](https://github.com/user-attachments/assets/fba4a59d-639e-465e-bb3b-c73514d0b3ec)


sha1 hash


command


hashcat -m 100 -a 0 sha1.txt rockyou.txt



The command above is a sha1 hash command. The mode 100 specifies the
hash wich is sha1 hash function. 


result of sha1 hash



combinator attack:








Mask attack:





How to defend against hashcat


1. stronger passwords
2. add salts to password hashes(salting)

To crack a salted password, the attacker should know both the hash and salted values. Thats why salting makes it harder for the attacker to crack the password.

Salting hash function Example:


![image](https://github.com/user-attachments/assets/2f7d3742-a57b-4d10-be3b-f67f7504dc73)

3. dynamic salting



summary


Hashcat is a very powerful tool that helps to crack password hashes. We also learned about mathamatical hash functions and how you can add salts to the hash functions. Lastly I showed you all how to crack diffrent hashing modes on hashcat.


   
























