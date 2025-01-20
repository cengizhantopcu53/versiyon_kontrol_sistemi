# Clone-repo

**Go to Project** <br>
- Open Terminal. Go to directory where the project will be saved. (eg. C:\Users\...\Projects\firma) <br> 
	
		cd  C:\Users\"your-username"\Projects\"group-name"

<br>

**Clone an Existing Repo** <br>
- Clone a repository to your local machine with repo url (SSH). SSH  will be obtained from the main menu of the repository on GitBucket.<br>
- From top-right of menu change HTTP to SSH and copy the link (eq. SSH  will be like this; ssh://git@gitserver.tr.local:29418/.../guide.git)<br>

		git clone "repo-url"

<br>

**Cloning specific History** <br>
- Belirli bir derinliğe kadar geçmişi olan bir kopya ile depo klonlama veya fetch işlemi yapmanıza olanak tanır. <br>
Bu, genellikle büyük depoları klonlarken zaman ve disk alanından tasarruf etmek için kullanılır.
- Argüman sonrasında gelen sayı, Git'in alacağı commit sayısını belirler.<br>

		git clone --depth 1 <repo-url>

<br>

**Regularly Update your Clone** <br>
- You got the project in your local machine. To update project file in your local machine 
(which means that somebody make changes in different machine and you take final verison of the project to your machine).<br>
- This command should be made regularly to avoid confusion.<br>

		git pull

