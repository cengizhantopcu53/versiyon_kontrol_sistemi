# Stashing Changes

- Çalışma dizininizdeki değişiklikleri geçici olarak saklamanıza ve daha sonra geri yüklemenize olanak tanıyan bir Git komutudur. Özellikle üzerinde çalıştığınız bir şeyi bitirmeden farklı bir işe geçmeniz gerektiğinde veya hızlıca başka bir branch'e geçmek istediğinizde kullanışlıdır. 

<br>

**Çalışma dizinindeki değişiklikleri saklama**<br>
- Çalışma dizinindeki tüm değişiklikleri geçici bir alana saklar. Bu sayede, çalışma diziniz temizlenir ve farklı bir iş üzerinde çalışabilirsiniz.
    
        git stash

 <br>

 **Stash listesini görüntüleme**<br>
- Saklanan değişikliklerin listesini gösterir. Her saklama işlemi bir indeks numarasıyla ilişkilendirilir.

        git stash list

 <br>

 **Saklanan değişiklikleri geri yükleme ve stash'i silme**<br>
- En son saklanan değişiklikleri geri yükler ve stash'i siler.
- Eğer uygulama sırasında bir çakışma (conflict) olursa, değişiklikler stash listesinden kaldırılmaz.

        git stash pop

- Belirli bir stash'i geri yüklemek ve silmek için,

        git stash pop stash@{n}

 <br>

  **Sadece saklanan değişiklikleri geri yükleme**<br>
- En son saklanan değişiklikleri geri yükler.
- Değişiklikleri uyguladıktan sonra hala stash listesinde saklamak istediğinizde kullanışlıdır.

        git stash apply
    
-  Eğer birden fazla stash varsa,

        git stash apply stash@{n}

 <br>

 **Sadece saklanan stash'i silme**<br>
- En son saklanan stash'i siler. 
- Geri yüklemek istemediğiniz ve kalıcı olarak silmek istediğiniz durumlarda kullanabilirsiniz.

        git stash drop

- Belirli bir stash'i siler.

        git stash drop stash@{n}

 <br>