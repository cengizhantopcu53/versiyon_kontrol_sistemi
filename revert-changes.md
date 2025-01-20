# Reverting Your Changes

- Git'in en güzel yanlarından biri de yaptığınız herhangi bir değişikliği kolayca geri alabilmemizi sağlamasıdır. <br>

 <br>

**Son Commit Mesajını Düzeltmek**<br>
- Sadece son yapılan commit işleminizindeki mesajı düzeltmek için kullanılır.

		git commit --amend -m "değiştirilen commit mesajı"

 <br>

**Local Değişiklikleri Geri Almak**<br>
- Değiştirdiğiniz halinden memnun olmadığınız dosyadaki değişiklikleri geri alıp dosyanın son commit edilmiş haline geri dönmek istediğinde kullanılır.

		git checkout -- dosya1.md

**Belirli bir Commit'e Geçmek**<br>
- Belirli bir commit'e geçmiş olacaksınız. Bu durumda, projeniz o commit'in durumunu yansıtacaktır.

		git checkout commit-hash

- Geri dönmek için çalışmakta olduğunuz dala geçiş yapabilirsiniz.

		git checkout branch
 <br>

**Commit Edilen Bir Değişikliği Geri Almak**<br>
- Commit ettiğiniz herhangi bir değişikliği geri almak için kullanılır.
- Yapılan commiti geri almak için otomatik olarak yeni bir commit oluşturur ve geri alma işlemi bu commit sayesinde değişiklik tarihçesinde görünür hale gelir.

		git revert HEAD 
		
 <br>

**Commiti Silme**<br>
- Eğer bir commit'i silmek istiyorsanız ve bu commit'i zaten uzak bir depoya (remote repository) pushladıysanız, bu işlemi dikkatli bir şekilde yapmanız gerekir. 
- Commit'i silmek, diğer insanların da bu commit'i almış olmasını ve geçmişlerine eklemiş olmalarını engellemez. Bu, işbirliği yaptığınız diğer insanlarla uyumsuzluklara neden olabilir. Bu işlemi diğer ekibinizle iletişim kurarak ve işbirliği yaparak gerçekleştirmeniz önemlidir.
- Otomatik yeni bir commit üretmeden değişikliğinizi geri almanızı sağlar.

- En son commit'inizi siler.

		git reset --hard HEAD

- En son üç commit'inizi siler.

		git reset --hard HEAD~3

- Belirli commit'inizi siler.

		git reset --hard 03b1ccb
		
<br>

**Değişiklikleri Uzak Depoya Zorla Push Etme**<br>
- Uzak depodaki mevcut durumu sizin lokal durumunuzla eşleştirmenizi sağlar. 

		git push origin HEAD --force
