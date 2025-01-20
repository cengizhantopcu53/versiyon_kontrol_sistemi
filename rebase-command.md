# Rebase Command

- Bir branch'in commit geçmişini, başka bir branch'in commit geçmişiyle yeniden düzenlemek için kullanılan bir Git işlemidir. Bu işlem, genellikle commit geçmişini daha temiz ve düzenli tutmak için tercih edilir.
- Rebase işlemi genellikle dikkatli bir şekilde yapılmalıdır, çünkü commit geçmişini değiştirmek karmaşık hatalara neden olabilir. Bu nedenle, rebase işleminden önce dikkatlice düşünmek ve gerekirse bir yedek almak önemlidir.

<br>

**Selecting Branches**<br>
- Rebase işlemi yapmak istediğiniz branch'e geçiş yapın.

        git checkout target_branch 

<br>

**Merge Process**<br>
- Rebase işlemi yapmak istediğiniz hedef branch'i belirtin.

        git rebase source_branch

<br>

**Resolve Conflicts**<br>
- Eğer rebase işlemi sırasında conflict oluşursa, bu çakışmaları çözmeniz gerekecektir. Git size çakışmaları çözmeniz için talimatlar verecektir.

<br>

**Complete the Rebase**<br>
- Çakışma olmadan veya çakışmaları çözdükten sonra, rebase işlemini tamamlamak için

        git add conflicted_file
        git rebase --continue

<br>

**Aborting a Rebase**<br>
- Rebase işlemini iptal etmek için

        git rebase --abort

<br>

**Pushing to a Remote Repository**<br>
- Eğer çalıştığınız branch'ler uzak bir depo ile paylaşılıyorsa ve rebase işlemi başarılı olduysa,

        git push origin target_branch

<br>