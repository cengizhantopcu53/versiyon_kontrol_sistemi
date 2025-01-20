# Merge Changes

- Birleştirme işlemi, Git'te farklı branch'lerde yapılan değişiklikleri birleştirmek amacıyla kullanılan bir işlemdir. Bu işlem, bir geliştirme branch'inde yapılan değişiklikleri, genellikle ana branch veya başka bir hedef branch ile birleştirme anlamına gelir. 

<br>

**Merge Scenarios**<br>
- Git'te merge işlemi farklı senaryolarda gerçekleşebilir. Temel olarak merge durumları şunlardır:

**Fast-forward merge:** Bir branch, diğer branch'in tüm commit'lerini içeriyorsa ve bu commit'ler sonradan yapılan commit'lerden önce gerçekleşmişse, Git bu commit'leri doğrudan ileri alarak birleştirir. Bu durumda ek bir commit oluşturulmaz.<br>
**Automatic merge:** İki branch'in birleştirilmesi durumunda, Git otomatik olarak çakışmaları çözmeye çalışır. Eğer çakışma yoksa, birleştirme otomatik olarak gerçekleşir. Ancak, eğer çakışmalar varsa ve Git bu çakışmaları otomatik olarak çözemezse, bir conflict durumu oluşur ve manuel çözüm gerekebilir.<br>
**Manual merge**: İki branch birleştirilmek istendiğinde, aynı dosyanın aynı satırlarında farklı değişiklikler yapılmışsa veya dosya bir branch'te silinmişse, bir conflict durumu oluşur. Bu durumda, Git çakışmayı çözemediğinden kullanıcıdan manuel olarak çözüm yapması beklenir.

- Bu temel durumların dışında, bazen daha karmaşık merge senaryoları da oluşabilir, ancak genellikle bu üç durumu karşılaşılır.

<br>

**Selecting Branches**<br>
- Birleştirme işlemi yapılacak olan branch'leri seçmek için

        git checkout target_branch 

<br>

**Merge Changes**<br>
- Seçilen hedef branch'te, diğer branch'teki değişiklikleri birleştirmek için,

        git merge source_branch

- Bu komut, source_branch'deki değişiklikleri target_branch'e birleştirir.

<br>

**Dealing with Conflict Situations**<br>
- Eğer conflicts ortaya çıkarsa, Git bu durumu işaret eder. Çakışmaları çözmek için, dosyaları düzenleyip ardından çözümlenmiş dosyaları işleme eklemek için,

        git add conflicted_file
        git merge --continue

<br>

**Creating a Merge Commit**<br>
- Birleştirme işlemi başarıyla tamamlandığında, Git birleştirme işlemi için yeni bir commit oluşturur. Bu commit mesajı, otomatik olarak bir birleştirme mesajı içerir.

<br>

**Aborting a Merge Commit**<br>
- Eğer birleştirme işleminden vazgeçmek gerekiyorsa, yani merge commit'i iptal etmek istiyorsanız,

        git merge --abort

<br>

**Pushing to a Remote Repository**<br>
- Eğer çalıştığınız branch'ler uzak bir depo ile paylaşılıyorsa ve birleştirme işlemi başarılı olduysa,

        git push origin target_branch

<br>

**Commit Squashing**<br>
- Birden fazla commit'i tek bir commit olarak birleştirmek için kullanılan bir işlemdir. Bu işlem, özellikle bir feature branch üzerinde yapılan çok sayıda commit'i, ana branch'e merge edilmeden önce temizlemek için yararlıdır,

        git merge --squash





