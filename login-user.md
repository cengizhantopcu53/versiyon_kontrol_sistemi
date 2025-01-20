# Login User

**Setup**<br>
- Download Git from following link:<br>

		https://git-scm.com/downloads

<br>

**Config**<br>
- Open Terminal and type following commands:<br>
- Full name is your user name. <br>
- Email address will be *****@.com 

		git config --global user.name "Your-Full-Name"
		git config --global user.email "your-email-address"

- Check configuration informations with following command:<br>

		git config -l

<br>

**SSH**<br>
- Type the following for generating SSH key:<br>

		ssh-keygen -t rsa -b 4096 -C "your-email-address"

- Press enter three times for following prompts: <br>
- Enter a file in which to save the key (/c/Users/YOU/.ssh/id_ALGORITHM):[Press enter]<br>
- Enter passphrase (empty for no passphrase): [Type a passphrase]<br>
- Enter same passphrase again: [Type passphrase again]

-	To read your generated key type following command:<br>

			cat ~/.ssh/id_rsa.pub	

- Copy the outcome. 
- Open gitbucket from browser and login your account. 
- Click your image which is located top-right corner. 
- Select Account settings.
- Select SSH Keys. 
- Fill "Title" as your computer id. 
- Paste your key to "Key".
