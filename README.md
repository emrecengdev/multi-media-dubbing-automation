# Multi-media dubbing automation

Modern yapay zeka konuşma sentezi, günlük oluşturma, dil tanımlama ve ses klonlama kullanarak çok dilli medya  seslendirme programı.

## Projenin Amacı

Birçok dizi, film, haber bölümü, röportaj, sesli kitap ve video asla diğer dillere uygun dublajlanmayacak ve bir şeyi sıfırdan dublajlamak çok büyük bir girişim olabilir. Bu durum körlük, disleksi, öğrenme güçlüğü çeken ya da sadece altyazı okumaktan hoşlanmayan kişiler için yaygın bir erişilebilirlik engeli teşkil etmektedir. Bu program, bu zorluklarla karşılaşan insanlar için hoş bir alternatif yaratmayı amaçlamaktadır.


## Yapılacaklar
- Dil tespiti için daha iyi bir filtreleme sistemi. Belki kapsayıcı ve dışlayıcı veya güven eşiği
- Demoları herkese açık olarak görüntülemek için daha az telif hakkı olan çok dilli / İngilizce olmayan içerik bulun
- kullanıcının sadece İngilizce yerine hedef dilini seçebilmesi için anadilden arındırma
- PYDUB'IN APTAL ARRAY BOZUKLUĞUNU DÜZELTİN, böylece dublaj başına 5 IO işlemi yapmak zorunda kalmayalım!!!
- ~~orijinal hoparlörleri kaldırmak / hafifletmek için kaynak ses üzerinde bir vokal izolasyonu / sökücü çalıştırın?
- ~~Tüm platformlar için uygun bir kurulum kılavuzu~~
- bozuk espeak uygulamasını platformlar arası olacak şekilde kaldırın veya düzeltin
- ~~ Başlangıçta ağır modeller için başlatılmamış, tekli modeller (örneğin, yalnızca gerektiğinde pyannote/speechbrain boru hatlarını başlatın) ~~
- Bellek ayak izini azaltmak için aynı modeli kullanan tekil Coqui sesleri için soyutlama
- FFMPEG ile ses / altyazı akışlarını listelemek ve seçmek için ~~GUI sekmesi~~
- ~~Sekmeleri kendi sınıflarına taşıyın ~~
- ~~Tüm kontrollere etiketler ve ekran okuyucu işaretleri ekleyin ~~
- ~~Tek hoparlör veya çoklu hoparlör kontrol anahtarı ~~
- ~~ YouTube videosunu Altyazılı olarak indirin~~
- ~~Dublaj için başlangıç ve bitiş zamanını seçmek için kullanıcı arayüzü~~
- Web sitemde bir Flask sunucusu açın, böylece minimum özelliklerle deneyebilirsiniz.
- Alt akışı olmayan videolar için altyazı oluşturmak üzere OCR kullanın
- Metin tabanlı olmayan altyazılar için OCR kullanın
- Havalı bir logo mu yapıyorsunuz?
- Python programlarını ikili dosyalar olarak nasıl paketleyeceğinizi öğrenin
- ~~Telifli içeriği bu depodan kaldırın (üzgünüm üzgün değilim TV Tokyo)~~
- Yapılandırma dosyalarını daha sonra kullanmak üzere kaydedin ve içe aktarın
- ~~Tüm altyazı formatları için destek~~
- Belki altyazısız videolar için bir ASR kütüphanesi eklenebilir?
- Belki mıknatıs URL'leri veya korsan medya için arrLib desteği (kim bilir???)

### Günlükleştirme
- Liste kutusundan seçilen sese göre altyazıları filtreleme
- Birden fazla günlükleştirme modeli / boru hattı arasından seçim yapın
- Altyazı zamanlamalarına göre konuşma satırlarını izole ederek ses kayıtlarını diyarizayon için optimize edin
- Diart'ı araştırmak mı?

### TTS

- ~~Sesi hızlandırmak için PyDub kullanmak üzere hız kontrolünü yeniden düzenleyin~~
- ~~Hoparlörün ses seviyesini TTS ile eşleştirin~~
- Sıralı altyazı girişlerini ve küçük girişleri kaldırmak için onay kutusu, örneğin "nom" "nom" "nom" "nom"
- ses dönüşümünü araştırmak?
- Gerçekleştirilecek asenkron bir işlem kuyruğu oluşturun
- Started - Coqui model indirmeleri için asenkron GUI
- MyCroft Mimic 3 için destek ekleyin
- PiperTTS için Destek Ekleme

### Klonlama
- Altyazıları seçmek ve Coqui XTTS için bir veri kümesine veya wav derlemesine aktarmak için bir klonlama modu oluşturun
- Eğitim veri kümelerini izole etmek ve oluşturmak için günlükleri ve altyazıları kullanın
- Veri kümelerinin manuel olarak oluşturulmasını kolaylaştırmak için bir araç oluşturun

###### (oh tanrım, bu kelimenin tam anlamıyla çok fazla şey, bunun kapsamı çok büyüdü, bu nasıl bir şey olacak)

 
