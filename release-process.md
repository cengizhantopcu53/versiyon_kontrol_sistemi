# Releases Proceses

- Releases oluşturmak için yapılması gerek süreç anlatılmıştır.<br>
- Bu adımlar, bir projenin yeni bir sürümünü oluşturmak ve bu sürümü belgelendirmek için bir akışı temsil etmektedir. 
- Projenizde, pcb üretimi, müşteri testleri ve malzeme listesi ile pcb formunda güncellemeler yapıldığında version numaralandırması yapılması gerekiyor. Bu adımlar yapılmadan önce releases oluşturlması gerekir. 
- Releases paylaşılmadan pcb üretim yapılmamalı, müşteriye teste gidilmemeli ve satın almaya malzeme listesi ve pcb formu paylaşılmamalıdır. 

<br>

**1- Projenin Template Uygunluğunu Kontrol Etme**<br>
- Projenizin template uygun olduğunu doğrulayın. Template uygunluğu, proje dosyalarının ve yapılarının belirli bir standart ve düzen içinde olduğunu gösterir.

<br>

**2- Manufacturing Dosyalarını Güncelleme**<br>
- Projenin manufacturing dosyalarını güncelleyin. Manufacturing dosyaları, projemizin basta sonra uretilmesi icin gerekli uretim dosyalarını içeriyor.
- Üretimi yapılacak pcb'nin takibi için üzerine versiyon numarasının yazılması gerekir.

<br>


**3- Changelog Dosyasını Güncelleme**<br>
- Changelog dosyasını güncelleyin. Changelog, projenin hangi değişiklikleri içerdiğini, güncelleme veya sürüm notlarını içeren bir dosyadır. Bu dosya genellikle kullanıcılara ve geliştiricilere projedeki değişiklikleri anlatmak için kullanılır.
- Yayınlanacak sürümün tarihini yazmayı unutmayın. 
        
        v1.0-h1 dd.mm.yyy

<br>


**4- Release İçin Issue Oluşturma**<br>
- Yeni bir release için bir issue oluşturun. Bu isseu ile release oluşturmak için ekipten onay alınması gerekir. En az bir kişiden onay alınması için Assignee atamayı unutmayın.

- Örnek ıssue başlığı aşağıdaki gibi olmalıdır.

        Release Review: v1.0-h1

- Onay alındıktan sonra ıssue açılan kişi tarafından kapatılmalıdır. Onay alınmadan ıssue kapatılmamalı. 

<br>


**5- Git Tag Oluşturma**<br>
- Oluşturulan commit'e bir tag ekleyin. Bu etiket, sürüm numarasını veya sürüm adını içermelidir.

        git tag -a v1.0-h1 -m "v1.0-h1"

- veya belirli bir commit numarası için 

        git tag -a v1.0-h1 03b1ccb -m "v1.0-h1"

<br>


**6- Git Tag'leri Uzak Depoya Gönderme**<br>
- Oluşturulan etiketi uzak depoya göndermek için

        git push origin --tags

<br>


**7- GitBucket Üzerinde Release Oluşturma**<br>
- GitBucket web arayüzü üzerinden yeni bir release oluşturun. Bu işlem, projenizin belirli bir sürümünü tanımlamanızı sağlar.
- Create Release dedikten sonra bir kaç kelime ile oluşturulma nedenini yazınız.
