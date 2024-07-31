# Hashcat


Disclaimer: This is for educational purposes only.


Name: Rory Stiff



Decscription: Hashcat is a versatile hacking tool that assists brute force attacks 
by condcuting them with hash values of passwords. I will be showing md5 hashing and
sha56 hashing password techniques with hashcat and how to protect youurself from these attacks. 


Topics being covered

1. Whats Hashcat
2. whats password hashing
3. what is a hash function
4. what are md5 hashes/sha56 hashes
5. How to do a md5/sh56 sttack with hashcat
6. Mitigation steps to protect yourself


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

6 % 4 = 2

Table size = 4
index = 3



|------------|
|  0 index   |   
|------------|       
|  1 index   |       
|------------|
|   2 index  | -> <6> is stored at index 2
|------------|
|  3 index   |     
|------------|












