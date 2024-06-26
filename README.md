# SaveTree - Kitap Takas Web Projesi

![logo](https://github.com/12enes34/savetree/assets/102800363/af853869-224f-42ed-b934-65bc3bbb15f4)


## Proje Sahibi
**Enes Ünver**  

## Proje Amacı
Bu projeyi kitap üretimi için ağaçların kesilmesini engelleyerek doğayı korumak, aynı tür kitapları seven insanların birbirleriyle sosyalleşmesini sağlamak ve kitap okumak isteyen insanların daha fazla bilgi edinmesine katkıda bulunmak amacıyla geliştirdim.

## Proje Konusu
Kitap takas etmek isteyen insanların birbirleriyle kitaplarını takas edebileceği, herhangi bir çıkar amacı gütmeyen bir web sitesi geliştirmek.

## Kullanılan Teknolojiler ve Metodlar

- **PHP Mailer:** Kullanıcıların kayıt olurken ve şifrelerini sıfırlarken kullanabilecekleri e-posta doğrulama yöntemi.
- **Token Oluşturma:** Kullanıcı mailine token gönderme metodu.
- **Kullanıcı Adı Kontrolü:** Aynı kullanıcı adına sahip kullanıcıların olmasını engelleme.
- **Şifre Güvenliği:** Kullanıcı şifrelerinin belirli karakterleri içermesini sağlama ve SHA-256 ile şifrelerin korunması.
- **Veritabanı:** Kullanıcı ve kitap bilgilerini içeren kompakt ve hızlı yanıt veren veritabanı tasarımı.

## Veritabanı Yapısı

- **Kullanıcılar Tablosu:**
  - Kullanıcı Adı
  - Şehir Bilgisi
  - İsim, Soyisim
  - E-posta
  - Telefon Numarası
  - Şifre
  - Token Bilgisi

- **Kitaplar Tablosu:**
  - Sahip ID
  - Yazar Adı
  - Yayın Yılı
  - Yayın Numarası
  - Kitap İsmi
  - Kitap Türü

- **Takas Talepleri Tablosu:**
  - Takas İsteyen Kullanıcı ID
  - Takas Edilecek Kitap ID
  - Takas Onay Durumu

- **Takas Geçmişi Tablosu:**
  - Gerçekleşen takasların geçmişi ve kullanıcıya özel takas önerileri için kullanılır.

- **Geçici Token Tablosu:**
  - Sunucu içindeki geçici token bilgilerini tutar.

## Geliştirilmesi ve Eklenmesi Planlanan Özellikler

- **Sohbet:** Kullanıcıların birbirleri ile sohbet edebileceği bir platform.
- **Anlık Fotoğraf Çekme:** Kullanıcıların takas için kitap eklerken kameralarını kullanarak fotoğraf çekmeleri.
- **Fotoğraftan Kitap Adı Tanıma:** Yapay zeka kullanarak kitap adını fotoğraftan otomatik olarak tanıma.
- **Takas Kitabı Önerisi:** Kullanıcının önceki takaslarına dayanarak yeni kitap önerileri sunma.


## Ekran Görüntüleri

![Screenshot 2024-06-21 022755](https://github.com/12enes34/savetree/assets/102800363/e35f00ee-da34-4e3e-9fe1-e55d0724f5f3)
![Screenshot 2024-06-21 022849](https://github.com/12enes34/savetree/assets/102800363/5b56e624-c161-4cb5-bc97-5788a6bf371d)
![Screenshot 2024-06-21 022945](https://github.com/12enes34/savetree/assets/102800363/9306c434-5424-4bc8-9903-94816fefa5ee)
![Screenshot 2024-06-21 023024](https://github.com/12enes34/savetree/assets/102800363/dbaa2425-8140-4b27-8cb0-ce2e24f600c9)



## Lisans

Bu proje MIT lisansı ile lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakın.
