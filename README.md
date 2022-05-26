# Born2beRoot
Born2beRoot projesi için kullanılabilecek kaynaklar.

# Evaulation Soruları

## General instructions(Genel Talimatlar)

* Savunma sırasında, bir noktayı doğrulamak için yardıma ihtiyacınız olduğu anda, değerlendirilen öğrenci size yardımcı olmalıdır.
* "signature.txt" içindeki imzanın aynı olup olmadığını kontrol edin

## Mandatory part(Zorunlu kısım)

### Project overview(Projeye genel bakış)

Değerlendirilen öğrenci size basitçe şunları açıklamalıdır:

* Bir sanal makine nasıl çalışır.
* CentOS ve Debian arasındaki temel farklar.
* Sanal makinelerin amacı.
* Değerlendirilen öğrenci CentOS'u seçtiyse: SELinux ve DNF nedir.
* Değerlendirilen öğrenci Debian'ı seçtiyse:
aptitude ve apt arasındaki fark ve APPArmor nedir.

Savunma sırasında, bir komut dosyası tüm bilgileri göstermelidir.
her 10 dakikada bir. Çalışması daha sonra detaylı olarak kontrol edilecektir.
Açıklamalar net değilse, değerlendirme burada durur.

## Simple setup(Basit kurulum)

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacın olduğunda, değerlendirilen öğrenci
sana yardım edebilmelidir.

Root olmayan bir kullanıcı ile giriş yapın.
Seçilen şifreye dikkat edin, konuyla ilgili getirilen kurallara uymalıdır.
* Değerlendirici yardımıyla UFW hizmetinin başlatıldığını kontrol edin.
* Değerlendirici yardımıyla SSH hizmetinin başlatıldığını kontrol edin.
* Değerlendirici yardımıyla seçilen işletim sisteminin Debian veya CentOS olup olmadığını kontrol edin.

Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa, değerlendirme burada durur.

## User(Kullanıcı)

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacın olduğunda, değerlendirilen öğrenci sana yardım edebilmelidir.

Doküman, değerlendirilmekte olan öğrencinin oturum açma bilgilerine sahip bir kullanıcının sanal makinede mevcut olmasını ister.

Kullanıcının "sudo" ve "user42" gruplarına eklendiğini kontrol edin.

İlk olarak, yeni bir kullanıcı oluşturun. Dokümanda verilen kurallara uyarak istediğiniz şifreyi atayın.
değerlendirilmekte olan öğrenci şimdi size istenen kuralları nasıl ayarladığını açıklamalıdır.
Normalde bir veya iki değiştirilmiş dosya olmalıdır. Herhangi bir sorun varsa, değerlendirme burada durur.

* Artık yeni bir kullanıcınız olduğuna göre,değerlendirilmekte olan öğrenciden "evaluating" adlı bir grup oluşturmasını isteyin.
Kullanıcıyı bu gruba ekleyin. Son olarak, bu kullanıcının "evaluating" gruba ait olduğunu kontrol edin.

* Son olarak, değerlendirilmekte olan öğrenciden bu şifre politikasının avantajlarını ve dezavantajları anlatmasını isteyin.

Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa değerlendirme burada durur.

## Hostname and partitions(Ana bilgisayar ve bölümler)

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacınız olduğunda, değerlendirilen öğrenci
sana yardım edebilmelidir.

* Makinenin ana bilgisayar adının aşağıdaki gibi doğru biçimde biçimlendirildiğini kontrol edin:
login42 (değerlendirilen öğrencinin oturum adı).

*  Oturum açmayı sizinkiyle değiştirerek bu ana bilgisayar adını değiştirin, ardından makineyi yeniden başlatın.
Yeniden başlatıldığında ana bilgisayar adı güncellenmemişse değerlendirme burada durur.
* Artık makineyi orijinal ana bilgisayar adına geri yükleyebilirsiniz.
* Değerlendirilen öğrenciye bu sanal makine için bölümleri nasıl görüntüleyeceğini sorun.
* Çıktıyı dokümanda verilen örnekle karşılaştırın. Lütfen dikkat: eğer öğrenci bonusları yapmışsa bonus örneğine başvurmak gerekecektir.

Değerlendirilen öğrenci, LVM'nin nasıl çalıştığı ve neyle ilgili olduğu hakkında size kısa bir açıklama yapmalı.

Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa, değerlendirme burada durur.

## SUDO

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacın olduğunda, değerlendirilen öğrenci
sana yardım edebilmelidir.

* "sudo" programının sanal makineye düzgün şekilde yüklenip yüklenmediğini kontrol edin.
* Değerlendirilen öğrenci artık yeni kullanıcınızı "sudo" grubuna atadığını göstermelidir.
* Doküman, sudo için katı kurallar uygular. Değerlendirilen öğrenci öncelikle kendi seçtikleri örnekleri kullanarak sudo'nun değeri ve çalışmasını anlatmalıdır.
İkinci adımda, dokümanın getirdiği kuralların uygulanmasını size göstermelidir.
* "/var/log/sudo/" klasörünün var olduğunu ve en az bir dosyaya sahip olduğunu doğrulayın. İçeriği kontrol edin. Bu klasördeki dosyaların, sudo ile kullanılan komutların geçmişini görmelisiniz.
Son olarak, sudo üzerinden bir komut çalıştırmayı deneyin. "/var/log/sudo/" klasöründeki dosya(lar)ın olup olmadığına bakın.

Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa değerlendirme burada durur.

## UFW 

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacın olduğunda, değerlendirilen öğrenci
sana yardım edebilmelidir.

* "UFW" programının sanal makineye düzgün şekilde yüklenip yüklenmediğini kontrol edin.
* Düzgün çalışıp çalışmadığını kontrol edin.
* Değerlendirilen öğrenci size temel olarak UFW'nin ne olduğunu ve kullanmanın değeri açıklamalıdır.
* UFW'deki aktif kuralları listeleyin. 4242 numaralı bağlantı noktası için bir kural bulunmalıdır.
* 8080 numaralı bağlantı noktasını açmak için yeni bir kural ekleyin. Etkin kuralları listeleyerek bunun eklendiğini kontrol edin.
* Son olarak, değerlendirilen öğrencinin yardımıyla bu yeni kuralı silin.

Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa değerlendirme burada durur.

## SSH

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacın olduğunda, değerlendirilen öğrenci
sana yardım edebilmelidir.

* SSH hizmetinin sanal makineye düzgün şekilde yüklenip yüklenmediğini kontrol edin.
* Düzgün çalışıp çalışmadığını kontrol edin.
* Değerlendirilen öğrenci size SSH'nin ne olduğunu ve onu kullanmanın değerini temel olarak açıklayabilmeli.
* SSH hizmetinin yalnızca 4242 numaralı bağlantı noktasını kullandığını doğrulayın.
* Değerlendirilen öğrenci, yeni oluşturulan kullanıcı ile giriş yapabilmeniz için SSH kullanmanıza yardımcı olmalıdır.
Bunu yapmak için bir anahtar veya basit bir şifre kullanabilirsiniz. Değerlendirilen öğrenciye bağlı olacaktır.
Tabii ki konuda belirtildiği gibi "root" kullanıcısı ile SSH kullanamayacağınızdan emin olmalısınız.


Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa değerlendirme burada durur.

## Script monitoring

Unutmayın: Bir şeyi kontrol etmek için yardıma ihtiyacın olduğunda, değerlendirilen öğrenci
sana yardım edebilmelidir.

Değerlendirilen öğrenci size basitçe şunları açıklamalıdır:
* Size kodu göstererek komut dosyalarının nasıl çalıştığını.
* "Cron" nedir?
* Değerlendirilen öğrencinin senaryosunu sunucunun başladığı andan itibaren her 10 dakikada bir çalışacak şekilde nasıl kurduğu.
Senaryonun doğru işleyişi doğrulandıktan sonra, öğrenci değerlendirilmelidir.
Bu betiğin her dakika çalışmasını sağlamalıdır. 
Komut dosyasının dinamik değerlerle doğru şekilde çalıştığından emin olmak için ne istersen çalıştırabilirsin. *** Son olarak, değerlendirilen öğrenci sunucu başlatıldığında komut dosyasının çalışmasını durdurmalı, ancak betiğin kendisini değiştirme. *** Bu noktayı kontrol etmek için yeniden başlatmanız gerekecek sunucuya son bir kez Başlangıçta, komut dosyasının kontrol edilmesi gerekecektir. hala aynı yerde var olduğunu, haklarının değişmediğini ve
değiştirilmemiştir.

Bir şey beklendiği gibi çalışmıyorsa veya net bir şekilde açıklanmıyorsa değerlendirme burada durur.


# Kaynaklar

https://www.youtube.com/watch?v=0eTfvCXUv0A

https://www.debian.org.tr/Debian_Manifesto