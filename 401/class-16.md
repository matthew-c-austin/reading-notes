# Read: Class 14

## Reflections

This reading assignment talks about something that is interesting to me, but seems beyond my ken: passowrd hashing, salting, and encryption algorithms.

## Readings

[Intro to password hashing](https://auth0.com/blog/hashing-passwords-one-way-road-to-security/)

1. Define the term “hashing”.

    "Hashing" is the process of converting data (such as a password) into a fixed-length string of characters using a mathematical algorithm called a hash function. Hashing is a one-way operation, meaning that it is computationally infeasible to reverse-engineer the original data from the hash.

2. Explain to a non-technical friend what a hash function does to a password.

   A hash function takes a password and transforms it into a scrambled string of characters. This process is like putting a message through a secret code, where the output is unique to the input but nearly impossible to reverse back to the original password.

[bcrypt overview](https://danboterhoven.medium.com/why-you-should-use-bcrypt-to-hash-passwords-af330100b861)

1. What does it mean to ‘salt’ a password?

    'Salting' a password means adding a random value (the 'salt') to the password before hashing it. This technique increases the security of hashed passwords by making it more difficult for an attacker to use precomputed tables (rainbow tables) or guess the password using a brute-force attack.

2. What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?

    To find the 'salt' string for your passwords, a hacker would need to access the system or database where the salt values are stored, usually alongside the hashed passwords.

[jBCrypt](https://www.mindrot.org/projects/jBCrypt/)

1. How does the Blowfish block cipher handle the increased computation speed of new computers?

    The computation cost of the algorithm is parametised, so it can be increased as computers get faster.

2. What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?

     "Java password hash" and "Java password encryption" both offer terrible advice: one uses an unsalted hash which allows reverse dictionary lookup of passwords and the other recommends reversible encryption, which is rarely needed and should only be used as a last resort.

## Things I want to know more about

1. How much of this sort of knowledge would a backend engineer need to be intimately familiar with? Is the implementation something that infosec or ops would do, or would there be some requirements that the SDE needs to meet that is entirely up to them to match?
