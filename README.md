# h3-Hash


## € Schneier 2015: Applied Cryptography: Chapter 2 - Protocol Building Blocks: subchapters "2.3 One-way Fuctions" and "2.4 One-Way Hash Functions".

* The goal of cryptography is solve problems that can be caused by issues with authentication, lack of integrity, and dishonest people. Within this goal, there are definied protocols, e.g, series of steps that are used to guideline certain order of tasks.
* One-way function is a vital part of these protocols. One-way funtion, according to it's name, goes from one way to another without returning back. It is like me going to Japan for holiday and never coming back (ideal). One-way functions are not very good for encryption as there is no way to return it.
* One-way hash function is another part of protocols and a major part of modern cyrptography. It has many names of which I will not type in here.  Hash function takes input string of varying lengh and magically turns it fixed lenght output string. Hashing is the one-way act of converting the data (called a message) into the output (called the hash). Security-wise hash function is not secure. It is a public funtion and its secureness lies in the fact there is only one way to move. It is impossible to find the input data by checking output.

## Karvinen 2022: Cracking Passwords with Hashcat

* Article describes how to crack passwords with hashcat
* When trying to open the hash, it is important to know what type of hash is being opened. This can be done through comparison
* Opening the hash can be even faster with normal computer and it's local operating system. Virtual machine uses limited amount of GPU and with normal set-up, one gains speed boost.

* ![VirtualBox_DebianHeidi_08_11_2024_23_11_28](https://github.com/user-attachments/assets/946294b5-fa62-4df7-9c2e-26ffe2c33192)
* ![VirtualBox_DebianHeidi_08_11_2024_23_11_44](https://github.com/user-attachments/assets/aae6ed3f-f9a2-4f49-a153-f061c6adf052)

*Notes: It would be good if the instructions would state how to add the password: It did not seem to work for me until I googled and got the information that console does not show that you are typing in the password and you just need to know to type it and press enter. This is not clear to everyone but could be made more clear.


## Voluntary bonus article: Karvinen 2020: Command Line Basics Revisited

* Article describes basic functions of Linux command line and basic commands.
* This extra action for those who are not confident with systems used and langugage spoken.
* Tested few functions, worked OK albeit some challenges with screenshotting and keyboard combinations. What do you mean that ctrl+c/v does not work in this kind of command line?
![VirtualBox_DebianHeidi_08_11_2024_22_51_40](https://github.com/user-attachments/assets/42c8cd79-d310-4d7a-93e8-57f942ff3cd0)


##  Santos et al 2017: Security Penetration Testing - The Art of Hacking Series LiveLessons: Lesson 6: Hacking User Credentials (8 videos, about 30 min)


### a) Billion dollar busywork. Command 'echo -n "hello"|sha256sum' prints a hash. Try adding something to the string, e.g. 'echo -n 'hello asdf'|sha256sum'. What do you have to add to get a hash that starts with a zero? (Voluntary bonus: How is this related to Bitcoin? Voluntary difficult bonus: How many zeros can you get to the beginning? Voluntary difficult bonus: How does the difficulty raise?)


### b) Compare hash. Create a small text file. Take it's hash (e.g. 'sha256sum tero.txt'). Change one letter. Take the hash again. Compare hashes. What do you notice?



### c) Hashcat. Install hashcat and test that it works.

I installed hashcat and perfomed tests with it based on source materials.
![VirtualBox_DebianHeidi_08_11_2024_23_17_49](https://github.com/user-attachments/assets/dc5b75a9-e9cb-4dc3-84f3-73e682d49087)

![VirtualBox_DebianHeidi_08_11_2024_23_18_12](https://github.com/user-attachments/assets/e83c9926-c9e1-4209-b816-03ae1176729f)


### d) Dictionary attack. Crack this hash: 21232f297a57a5a743894a0e4a801fc3

I tried to do this according to instructions
![image](https://github.com/user-attachments/assets/adba5996-6240-4227-a9a2-cb6278e19e0e)

but was not able to crack the hash. Got the same error multiple times. There something wrong with my hash.
![VirtualBox_DebianHeidi_08_11_2024_23_21_49](https://github.com/user-attachments/assets/d3a7ca8a-b390-4ce5-a2c6-8ef7e8ab7627)
![VirtualBox_DebianHeidi_08_11_2024_23_25_56](https://github.com/user-attachments/assets/113289df-2078-4c11-a94e-2dedf7f32ba6)



### e) How can you make a password that's protected against a dictionary attack?

### Feedback

Thank you for listening to our comments on the amount feedback. I was not borderline crying with stress this time like I was during homework 2. This homework took around 6 hours to complete.

### References
https://www.howtogeek.com/devops/how-to-protect-your-organization-against-password-dictionary-attacks/


