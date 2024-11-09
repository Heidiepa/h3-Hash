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


### a) Billion dollar busywork. Command 'echo -n "hello"|sha256sum' prints a hash. Try adding something to the string, e.g. 'echo -n 'hello asdf'|sha256sum'. What do you have to add to get a hash that starts with a zero? (Voluntary bonus: How is this related to Bitcoin? Voluntary difficult bonus: How many zeros can you get to the beginning? Voluntary difficult bonus: How does the difficulty raise?)

I was unfortunately not able to get any results of this task. I tried writing in instructed command multiple times but it did not yield any results. I only got error "command not found"

![VirtualBox_DebianHeidi_09_11_2024_00_00_42](https://github.com/user-attachments/assets/feb6f019-7aee-4ecd-8f81-189a1390ff3e)
![VirtualBox_DebianHeidi_09_11_2024_09_44_51](https://github.com/user-attachments/assets/c87b8579-9445-49ed-a6be-e5b13400c318)

With horrible success in the the task, I did try the second task expecting failure and that is what is got! Again, "command not found"
![VirtualBox_DebianHeidi_09_11_2024_09_50_01](https://github.com/user-attachments/assets/f368e62a-4097-4837-a137-59ce9f4712ea)

I don't know what to add to get hash that starts with zero.

#### Voluntary bonus: How is this related to Bitcoin?
If I can guess, I think it relates to hashrate Bitcoin has. Hashrate is a securitey measurement in Bitcoin. The more there is power, the more secure Bitcoin is to attacks. Xurrent hashrate is around 750-780 TH/s. (Bitcoin)

### b) Compare hash. Create a small text file. Take it's hash (e.g. 'sha256sum tero.txt'). Change one letter. Take the hash again. Compare hashes. What do you notice?

I don't understand waht should be done it here. Should I have crated a small text file in where? Inside my virtual machine? And should I still have the github link library on to do this? Or should I have restarted the whole terminal?

Even if I don't know what to do, I expect that changing hash a by one letter will change the values as well. Some of the information will stay as it is though. And changing more letters will change the values more?

### c) Hashcat. Install hashcat and test that it works.

I installed hashcat and perfomed tests with it based on source materials. BGot it working through basic information.
![VirtualBox_DebianHeidi_08_11_2024_23_17_49](https://github.com/user-attachments/assets/dc5b75a9-e9cb-4dc3-84f3-73e682d49087)

![VirtualBox_DebianHeidi_08_11_2024_23_18_12](https://github.com/user-attachments/assets/e83c9926-c9e1-4209-b816-03ae1176729f)


### d) Dictionary attack. Crack this hash: 21232f297a57a5a743894a0e4a801fc3

I tried to do this according to instructions (changing value to be hashed)
![image](https://github.com/user-attachments/assets/adba5996-6240-4227-a9a2-cb6278e19e0e)

but was not able to crack the hash. Got the same error multiple times. There something wrong with my hash. I attempted this multiple times during the day and night (also restarted the hashing three times) and always got the same result. I expect something to be wrong but I don't know how to resolve this.
![VirtualBox_DebianHeidi_08_11_2024_23_21_49](https://github.com/user-attachments/assets/d3a7ca8a-b390-4ce5-a2c6-8ef7e8ab7627)
![VirtualBox_DebianHeidi_08_11_2024_23_25_56](https://github.com/user-attachments/assets/113289df-2078-4c11-a94e-2dedf7f32ba6)'
![VirtualBox_DebianHeidi_09_11_2024_09_38_03](https://github.com/user-attachments/assets/1bcfb716-1b50-4799-8e32-cf06ac711f06)

### e) How can you make a password that's protected against a dictionary attack?

### Feedback

Thank you for listening to our comments on the amount feedback. I was not borderline crying with stress this time like I was during homework 2 and it is a relief.

### References
https://www.howtogeek.com/devops/how-to-protect-your-organization-against-password-dictionary-attacks/

Bitcoin. Hashrate.
Mining hashrate is a key security metric. The more hashing (computing) power in the network, the greater its security and its overall resistance to attack.


