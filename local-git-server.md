# Local git Server

- [Türkçe](https://serdarsari.dev/windows-kendi-git-servisinizi-kurun-detayli-anlatim-turkce/) ve [yabancı](https://www.anchorpoint.app/blog/how-to-set-up-a-local-git-server-on-windows-in-10-minutes-using-gitea) kaynaklardaki talimatları inceleyerek kendi yerel git serverınızı kurabilirsiniz.

    - Gitea'nın [web sitesine](https://about.gitea.com/products/gitea/) gidin ve Windows sürümünü indirin.
    - Windows makinenizde tüm içeriklerin bulunacağı bir klasör oluşturun. Bu, tüm dosyaları, veritabanını ve Gitea sunucusunu içerir. Bir sonraki adımda, indirdiğiniz yürütülebilir dosyanızı bu klasöre taşıyın.
    - Yürütülebilir dosyayı çalıştırın. Bu bir komut satırı uygulaması açacaktır. Web tarayıcınızı localhost sayfasında açmak için Ctrl-tıklayın.
    - Veritabanı türü için "SQLite3"ü seçin çünkü herhangi bir yapılandırma olmadan yeni bir veritabanı oluşturacaktır. Gitea temel URL'niz için localhost yerine IP adresinizi girin. Bu, sunucunun ağınızdaki diğer bilgisayarlardan erişilebilir olması için gereklidir. Ardından "Gitea'yı Yükle"ye tıklayın ve oturum açma ekranına gelene kadar bekleyin.