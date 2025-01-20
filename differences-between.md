# Differences Between

- Git'te iki commit arasındaki farkları incelemek için git diff komutu kullanılır. Bu komut, iki commit arasındaki değişiklikleri gösterir, hangi satırların eklendiğini veya çıkarıldığını belirtir.

<br>

**Son Commit ile Çalışma Dizinindeki Değişiklikler Arasındaki Farkları Görüntüleme**<br>

        git diff

<br>

**İki Belirli Commit Arasındaki Farkları Görüntüleme**<br>
- Burada commit1 ve commit2, karşılaştırmak istediğiniz iki commit'in hash değerleridir veya başka bir şekilde referans gösterilebilirler (örneğin, branch isimleri, HEAD, HEAD~1 gibi)

        git diff commit1 commit2

<br>

**Belirli Bir Dosyadaki Değişiklikleri Görüntüleme**<br>
- Bu komut, yalnızca belirtilen dosyadaki değişiklikleri gösterir.

        git diff commit1 commit2 -- dosya_yolu

<br>

**İki Farklı Branch Arasındaki Farkları Görüntüleme**<br>

        git diff branch1 branch2

<br>

**Değişikliklerin Özetini Görüntüleme (Hangi Dosyaların Değiştiğini Gösterir)**<br>

        git diff --stat commit1 commit2

<br>

**Bir Dosyada Hangi Satırların Değiştiğini Görüntüleme**<br>
- -U0 seçeneği, değişikliklerin etrafında hiçbir bağlam satırı göstermez, yalnızca değişen satırları gösterir.

        git diff -U0 commit1 commit2 -- dosya_yolu

<br>