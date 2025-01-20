# Cherry-Pick Commit

<br>

**Başka bir daldaki belirli bir commit'i mevcut dala uygulama**<br>
- Belirli bir commit'i mevcut çalışma dalına uygulamanızı sağlayan bir yöntemdir. Bu işlem, seçilen commit'teki değişiklikleri alıp mevcut dalınızın üzerine yeni bir commit olarak ekler. 
- Bir hata düzeltmesi yalnızca bir dalda yapılmışsa ve bu düzeltmeyi başka bir dala uygulamak istiyorsanız kullanabilirsiniz.

        git cherry-pick <commit-hash>

- Örneğin, feature dalında yapılan bir değişikliği main dalına almak istiyorsunuz, ancak tüm feature dalını birleştirmek istemiyorsunuz. Bu durumda, cherry-pick komutunu kullanarak sadece istediğiniz commit'i main dalına uygulayabilirsiniz:


        git checkout main
        git cherry-pick <commit-hash>

- Burada commit-hash uygulamak istediğiniz commit'in hash değeridir. Bu işlem, belirtilen commit'in değişikliklerini içeren yeni bir commit oluşturur ve mevcut dalınıza ekler.

- cherry-pick işlemi, sadece belirli değişiklikleri almak istediğinizde kullanışlıdır, ancak bu işlem sırasında çakışmalar (conflicts) oluşabilir ve bunları manuel olarak çözmeniz gerekebilir. Ayrıca, cherry-pick kullanarak alınan değişiklikler, asıl commit'in bağlamından izole edilmiş olacağından, dikkatli kullanılmalıdır.
