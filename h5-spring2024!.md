# H5 - Spring 2024!

### x) Read or watch and summarize (This subtask x does not require tests with a computer. Some bullets per article is enough for your summary, feel free to write more if you like)
[€ Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions](https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003)

### a) Install Hashcat. Test it with a sample hash. See Karvinen 2022: Cracking Passwords with Hashcat
### b) Crack this hash: 8eb8e307a6d649bc7fb51443a06a216f
### c) Choose a password manager. (This subtask b does not require tests with a computer). First, create a short list of some password managers; then pick one. Explain:
#### A list of some well known password managers: Dashlane, Bitwarden, Google, 1Password, Nordpass

I chose Bitwarden due to having used it myself for around half a year now.

#### What threats does it protect against?
Bitwarden like any other password manager mainly protects agains threats relating to password security such as data breaches, unauthorized access, and phising.
  
#### What information is encrypted, what's not?
Bitwarden encrypts all the sensitive information added into the vault: passwords, credit card numbers, secure notes and any other personal information. They have a full list shown on their website [URL: https://bitwarden.com/help/vault-data/](https://bitwarden.com/help/vault-data/). What it does not encrypt is the metadata, as an example information regarding the names or structures of folders. This enables them to have different features regarding searching and organizing within their application. 
  
#### What's the license? How would you describe license's effects or categorize it?
Bitwarden is licensed under the GNU Affero General Public License version 3 (AGPLv3), it's a copyleft license. [Copyleft licensing](https://bytescare.com/blog/difference-between-copyright-and-copyleft) is a method that encourages the unrestricted sharing, modificication, and utilisation of all creative works. It ensures that the source code of the software is open and accessible to all users.
  
#### Where is the data stored? If in "the cloud", which country / juristiction / which companies? If on local disk, where?
They have data storage both on their own servers and on your local machine. For their own servers, they process and store all vault data in the Microsoft Azure Cloud in the US or EU. For local host, decrypted data is stored in memory only and never written to persisten storage. Encrypted data is stored in different locations regarding your operating systems. For Windows which I am using it would be here:
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/c68c5e82-3674-4c80-af93-6e6d8366ed36)
 
#### How is the data protected?
  The data is sealed with end-to-end AES-256 bit encryption, salted hashing, and PBKDF2 SHA-256 authentication process. The data is encrypted before it leaves your device, and the only person with access to decrypting it will be you, even the staff can't unlock your data. 
  
### d) Demonstrate the use of a password manager, the one you picked in previous subtask.

First step: Go to their website, there you can see the icon "Get started" in the right side menu and click that
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/b8d150ca-d488-4f5b-a4d1-a5b3e296936e)

Then: Set up your account
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/57b9d9b1-cd7c-41df-b5e3-3596802c8df7)

