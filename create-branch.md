# Branch-Creating

- Branches allow you to work on different parts of a project without impacting the master branch.
- When the work is complete, a branch can be merged with the main project. <br>
- You can even switch between branches and work on different projects without them interfering with each other. <br>

 <br>

**Go to Directory**<br>
- Open Terminal. Go to directory where the project will be saved. (eg. C:\Users\sinneci\Projects\cemsan\su-isitici) <br>
	
		cd  C:\Users\"your-username"\Projects\"group-name"\"project_name"

- (Optional) Check your current branch <br>
	
		git branch 
 <br>

**Create Branch**<br>
- Create a branch (use "-" as spaces between words. All will be in lower case) <br>
	
		git branch "branch-name"

- (Optional) Check all branches and ensure that you created a new one.<br>

		git branch -a

 <br>

**Switch to Branch**<br>
- Switch to this branch (to return previous branch : git checkout -) <br>

		git checkout "branch-name"

 <br>

**Push Branch**<br>
- Push this branch <br>

		git push --set-upstream origin "branch-name" 

 <br>

**Delete a Branch**<br>	
- Delete this branch <br>

		git branch -d "branch-name"

- Now you can apply repo-procedure to this branch.

 <br>

**Branch Naming**<br>	
- Git için bir branch oluştururken isim verme konusunda kesin bir kural yoktur, ancak iyi bir dal ismi vermenin bazı yaygın uygulamaları vardır:

	- **Açıklayıcı Olun**: Dalınızın amacını açıkça belirten bir isim seçin. Örneğin, bir özellik ekliyorsanız, özelliğin adını kullanabilirsiniz (feature/login-system)<br>
	- **Kısa ve Öz Olun**: Dal isimlerini mümkün olduğunca kısa ve öz tutun. Uzun isimler yazmak ve hatırlamak zor olabilir.
	- **Küçük Harf Kullanın**: Genellikle dal isimlerinde küçük harfler kullanılır. Büyük harfler, bazı durumlarda işletim sistemleri arasında sorunlara neden olabilir<br>
	- **Ayırıcı Olarak Taksim İşareti (/) Kullanın**: Dal isimlerinde kategoriler veya hiyerarşi oluşturmak için taksim işareti kullanabilirsiniz. Örneğin, feature/login-system, bugfix/login-error gibi<br>
	- **Numaralandırma Yapın**: Birden fazla dal aynı özelliği veya konuyu ele alıyorsa, sonlarına bir numara ekleyerek ayırt edebilirsiniz (feature/login-system-1, feature/login-system-2)<br>
	- **Kişisel Dal İsimleri**: Eğer bir ekibin parçasıysanız ve kişisel bir dal oluşturuyorsanız, dal isminin başına kendi kullanıcı adınızı veya kısaltmanızı ekleyebilirsiniz (john/feature/login-system)<br>