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
Next up: Download the mobile app, set up a local server on your computer or download the browser extension. In this case I've downloaded the browser extension (I also own the mobile version).
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/6f659c86-2102-4bb9-9548-e023953e2f9b)
Now you should see bitwarden in your extensions, you can pin it as an extension in which case it'll always show up on the right side as seen in the picture.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/bc7f179a-2996-47d8-a686-2468f622f2c9)

When you open up the extension you can see the following types.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/e452d2a1-6f05-4e2e-b6d2-f6923ea81a77)

I've used bitwarden mainly for passwords so I'll show a quick little setup for how to setup a password for a website.
You can add a password by clickling the little + icon on the right side.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/3dbe8f44-41c3-4b39-a399-c54ea752e630)

It'll pop up with this image, usually taking on the URL that the website is currently on, it can also be manually changed if wanted.
You can change the name of the save to whatever you like as long as the URL is written in the URL section. Make it whatever makes it the easiest to find for you. Then fill the username and password.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/70d80e65-0a84-4e63-afcc-077cfa701a65)

When setting up the password the app recommends that you use their password generator. In here you can choose the length and what kind of characters you'd want in your password.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/3e695ff8-b13e-43e0-a070-8522c60c18db)

One you're ready you can click on save.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/6130810c-c49f-4200-b23f-2aadc95dfb08)

Now whenever you're on the website it should show you an option for the password you just set up. By clicking on it, it should autofill the information, if that doesn't happen you can also click on the little icons with which you can manually copy the information into the needed boxes.

![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/828f7eb6-9c00-4bfb-bf35-df5464c53515)
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/da856981-1fd4-4817-9c44-4e17bdb8f34a)



