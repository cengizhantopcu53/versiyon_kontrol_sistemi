# Create Tag

- Reponuzda git üzerinden ara versiyonlar veya ana versiyonlar yayınlayabilirsiniz.

<br>

**Create Tag** <br>

- Version oluşturmak için,

        git tag "version-name"

<br>

**Creating an Annotated Label** <br>

- Açıklamalı version oluşturmak için,

        git tag -a "version-name" -m "Release version-name"

<br>

**Tagging a Specific Commitment**

- Belirli bir commit numarası eklemek için,

        git tag -a "version-name" "commit number" -m "Release version-name"

<br>

**Viewing a Specific Tag** <br>

- Belirli bir versiyonun ayrıntılarını görüntülemek için,

        git show "version-name"

<br>

**Deleting a Tag** <br>

- Bir etiketi silmek için,

        git tag -d "version-name"

<br>

**Sharing Tags in Remote Storage** <br>

- Oluşturulan etiketleri uzak bir depoya göndermek için,

        git push origin --tags

- veya <br>

        git push origin "version-name"

<br>

**List All Tags** <br>

- Oluşturulan tüm etiketleri listelemek için,

        git tag