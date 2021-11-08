---
published: true
---
## Week 11 Password Security

<dl>
  <dt>Passwords are one of the three forms of authentication, namely, what you know (along with what you have and what you are). Passwords are used almost everywhere as the first line of defense against unauthorized access to certain resources. Password-based authentication was first used in 1961 at MIT [source].

In this room, we explain what password hashing is, types of attacks carried out against passwords, defense methods, and some advice on how to mitigate the risks of password leaks.

Let us first define what password hashing is and some of the common hashing algorithms used. We will go into further depth in Task 6 but it is important to understand the basics first.

When a password is hashed, a one-way hashing algorithm function is performed on a password that generates a fingerprint or representation of the provided password, which we then identify as the hash. One-way hashing functions are generally easy to compute. However, the computation required to obtain the original input (plaintext password in this case) could be difficult and time-consuming, depending on the algorithm.</dt>
  
  
  <dd>Online vs offline attacks:</dd>
  

  <dt>In an online attack, password guessing can be largely defended against using some form of timeout between each entry or even some more extreme measure, by denying access to the account after an x number of attempts.</dt>
  <dd>In an offline setting, however, password guessing is much more accessible due to the dedicated hardware and advanced methods. This could be used by attackers that have obtained a database dump of usernames and passwords. Since the attack is carried out offline and without any intervention from the victim(s), this type of attack is almost impossible to defend against. However, this attack could be mitigated. 
</dd>
  
  
  
  <dd>Before we look at some statistics related to password length, let's first talk about password attack complexity. A brute-force attack grows exponentially with increasing key size. What does this mean? I won't bore you with all the details, but a small explanation won't hurt.

Say we have a function f(x) = 2x , this function grows exponentially fast. How fast is that growth? Very fast! Let us look at a small example. For instance, to go from 22 = 4 to 23 = 8, requires us double the work. The same logic applies when you go from 237 to 238 for example. Why double the work?  Because the number 2 is the base of the function. If the function was to be, f(x) = 3x, then it would require us triple the amount of work to go from 3x to 3x+1 and so on. So if you were to have a password with a key size of a certain length, you could always calculate how long a brute-force attack will take against your password (more on this later).

We just saw how every number requires the attacker to put double (or triple or even higher, depending on the base) the work in a brute-force attack. You may be wondering, are all attacks against passwords exponential in complexity? Certainly not! In the next task, we introduce attacks with lower complexity (= faster to carry out), based on neat mathematical tricks and doing a ton of pre-computations.
</dd>
  
  
  <dd>Based on 10-16 character words from the dictionary: The Oxford English dictionary has 218,632 (including obsolete words) 218. This even includes words that are less than 10 characters in length which stands no chance against an offline attack.
Obfuscated words: The user picks a random 10-16 character word from a dictionary and applies some pseudo transformations (e.g. leetspeak). For example, dictionary d1c71on4ry. The Oxford English dictionary has 218 words * 212 (leetspeak extra chars)  230.This does make your passwords harder to guess, but it is still in the danger zone when it comes to offline attacks.
What about the Diceware method? Which is simply picking a number of words from a certain list of words. Say we have 7776 (= 65) words to choose from. Then choosing 3 words results in 77763  239 Which is quite small. 4 words are already better 77764 252 . 6 words is getting us somewhere 77766 278. This is however still easy to enumerate using words from the dictionary.
Generating a password from a certain set of characters: Say a user generates a password randomly from the following set of characters: </dd>
  <dd> In the Jupyter notebook, run the cell in the Enable Document AI section to find out the active account email address. This is who the notebook user is running as. Copy this email address.</dd>
 
  <dt>No matter how complex a password is, how robust a hashing algorithm is, with unlimited (or at least sufficient) computing power or storage any password is breakable. 
An attacker would most likely prefer to steal a password in transit form for unencrypted login pages, through keylogging, via phishing, etc. However, if that is not possible, the attacker could still get their hands on passwords using some of the various methods below.
</dt>


  <dd>  Storing hashed passwords: Store the username and the derived key (hashed password) in a database: DK = hashFunction(Password). While this is better than storing passwords in plain text, it still has a lot of weaknesses. As the same password hashes to the same derived key. An attacker can pre-compute or download a large password/hash table and use it to look up passwords easily! For example, a password made from English words is 218 * 8Bytes ~ (~ means approximately) 2MB file. In other words, if an attacker were to compute a list of password hashes of each word in the English dictionary, this would result in a 2MB file and they just need to look up whether a certain password hash is in their list. 8 characters from [a-z] is 268 = 238 * 8Bytes ~ 2.2 terabyte of pre-computation storage is needed for near-instant lookup. 10 characters [a-zA-Z] is 5210 = 257 * 8Bytes ~ 1.6 exabyte ( 1 exabyte is equal to 1 million terabytes) of pre-computation storage is needed.
</dd>

  
  
  
 
 
</dl>

