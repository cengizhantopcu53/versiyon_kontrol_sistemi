# Remote Repositories

- Uzak depo, genellikle internet üzerinde veya ağınızda bulunan ve projenizin bir kopyasını tutan bir depodur. <br>
Yerel depo (local repository) ve uzak depo (remote repository) arasında kod paylaşımı yapılabilir.

<br>

**Uzak Depo Adresini Öğrneme** <br>
- Projenizle ilişkili tüm uzak depoların listesini ve her biri için fetch (çekme) ve push (itme) adreslerini gösterir. 
- Genellikle, varsayılan uzak depo adı "origin"dir ve bu komut size "origin" ile ilişkilendirilmiş URL'yi gösterecektir.  

        git remote -v
        
        origin  https://github.com/kullaniciadi/projeadi.git (fetch)
	origin  https://github.com/kullaniciadi/projeadi.git (push)

<br>

**Uzak Depo Eklemek** <br>
- Yeni bir uzak depo ekler ve bu depoya bir isim verir.

        git remote add <isim> <url>
        
        git remote add origin git@github.com:kullaniciadi/proje.git

<br>

**Uzak Depo Adresini Değiştirmek** <br>
- Belirtilen uzak deponun URL'sini değiştirir. 

        git remote set-url <isim> <yeni_url>
        
        git remote set-url origin git@github.com:kullaniciadi/yeniproje.git

<br>

**Uzak Depoyu Silmek** <br>
- Belirtilen uzak depoyu siler. 

        git remote remove <isim>
        
        git remote remove origin 

<br>
