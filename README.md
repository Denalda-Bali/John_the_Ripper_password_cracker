# John the Ripper Password Cracker

###### I will use John the Ripper to attempt to decipher the passwords from the hash files.

The purpose of the attack is password detection which is protected by hash algorithms.

I will create a hash file using the SHA256 hash algorithm.

Which assumes that the file holds a secret (password, phrase, ID, etc.) which could be for example the user password on a machine.

That file is taken and put under attack using John the Rripper.

## Step 1

The simplest way to create a hash file is by using the SHA256 hash function generator which generates a SHA256 hash (encoded SHA256) containing 64 hexadecimal digits. Which can be used as a password to protect data like money transactions, personal information etc ..

In my case, I am using an online tool that helps me generate a hash of an x ​​password in the SHA256 algorithm. Below will be the tool link.

> https://xorbin.com/tools/sha256-hash-calculator

## Step 2

After generating the hash, we place it in a text file.
In my case I called it Test.txt

We can control the hash type via Kali Linux by going to:
> Applications >> Password Attacks >> offline Attacks >> hash-identifer

Where we simply paste the hash that we generated before.

## Step 3

Open the terminal, and apply the following commands

> cd Desktop

Then we create a hash file using the following commands (setting a name what we want in my case Test-hash.txt)
in this file we put the generated hash code and save it.

> sudo nano Test-hash.txt

As we save the file it will appear on the desktop.

## Step 4

Then we use a wordlist (see command below), where it tries to break the password hashes in the given file (Test-hash.txt)
