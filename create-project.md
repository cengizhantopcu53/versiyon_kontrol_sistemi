# Create Project

**Create Repository on Github** <br>
- Open Github from browser and login your account. 
- Click "plus" icon which is located top-right corner near your image.
- Choose owner as the group this repo will be belong to. 
- Then enter Repository name (use "-" as spaces between words. All will be in lower case)
- "Private" and "Create an Empty repository" should be checked. 
- Then create the repository.

 <br> 

**Create Folder and Initialize Git** <br>
- Open Terminal. Go to directory where the project will be saved. (eg. C:\Users\ctopcu\Projects\firma\proje) <br>

		cd C:\Users\"your-username"\Projects\"group-name"\"project_name"

- For 3d-model <br>

		cd  C:\Users\Public\3d-model

- Initialize the git repository to this file	<br>

		git init

- Create following files to your project	<br>

		mkdir Documentation <br>
		mkdir Firmware  <br>
		mkdir Hardware	<br>
		mkdir Source <br>

 <br> 

**Add README file** <br>
- Create the Read Me file of your project	<br>

 		cd > README.md


- Check current status of your git (current branch, commits and untracked files)<br>

		git status

- Add Read Me file to your track<br>

		git add README.md

- Check status (README.md should appear in the "changes to be committed" part.)	<br>

		git status

 <br> 

**Commit README file** <br>
- Commit your README.md file to your project<br>

		git commit -m "First Commit"	

 <br> 

**Remote** <br>
- Connect your repo with repo url (ssh) with following command. Repo url  will be obtained from the main menu of the repository on GitHub<br>
- From top-right of menu change HTTP to SSH and copy the link (eq. SSH  will be like this; ssh://git@gitserver.tr.local:29418/.../guide.git)<br>

		git remote add origin "Your-SSH"

- Then push with following command<br>

    	git push -u origin master
