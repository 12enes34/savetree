# SaveTree - Kitap Takas Web Projesi / Book Exchange Web Project

![logo](https://github.com/12enes34/savetree/assets/102800363/af853869-224f-42ed-b934-65bc3bbb15f4)

## Proje Sahibi / Project Owner
**Enes Ünver**  

## Proje Amacı / Project Purpose
Bu projeyi kitap üretimi için ağaçların kesilmesini engelleyerek doğayı korumak, aynı tür kitapları seven insanların birbirleriyle sosyalleşmesini sağlamak ve kitap okumak isteyen insanların daha fazla bilgi edinmesine katkıda bulunmak amacıyla geliştirdim.  
I developed this project to prevent trees from being cut down for book production, to protect nature, to enable people who love the same type of books to socialize with each other, and to contribute to people who want to read books to gain more knowledge.

## Proje Konusu / Project Topic
Kitap takas etmek isteyen insanların birbirleriyle kitaplarını takas edebileceği, herhangi bir çıkar amacı gütmeyen bir web sitesi geliştirmek.  
Developing a non-profit website where people who want to exchange books can exchange their books with each other.

## Kullanılan Teknolojiler ve Metodlar / Technologies and Methods Used

- **PHP Mailer:** Kullanıcıların kayıt olurken ve şifrelerini sıfırlarken kullanabilecekleri e-posta doğrulama yöntemi.  
  An email verification method that users can use when registering and resetting passwords.
- **Token Oluşturma:** Kullanıcı mailine token gönderme metodu.  
  Method for sending tokens to the user's email.
- **Kullanıcı Adı Kontrolü:** Aynı kullanıcı adına sahip kullanıcıların olmasını engelleme.  
  Preventing users from having the same username.
- **Şifre Güvenliği:** Kullanıcı şifrelerinin belirli karakterleri içermesini sağlama ve SHA-256 ile şifrelerin korunması.  
  Ensuring that user passwords contain certain characters and protecting passwords with SHA-256.
- **Veritabanı:** Kullanıcı ve kitap bilgilerini içeren kompakt ve hızlı yanıt veren veritabanı tasarımı.  
  A compact and fast-responding database design containing user and book information.

## Veritabanı Yapısı / Database Structure

- **Kullanıcılar Tablosu / Users Table:**
  - Kullanıcı Adı / Username
  - Şehir Bilgisi / City Information
  - İsim, Soyisim / Name, Surname
  - E-posta / Email
  - Telefon Numarası / Phone Number
  - Şifre / Password
  - Token Bilgisi / Token Information

- **Kitaplar Tablosu / Books Table:**
  - Sahip ID / Owner ID
  - Yazar Adı / Author Name
  - Yayın Yılı / Publication Year
  - Yayın Numarası / Publication Number
  - Kitap İsmi / Book Name
  - Kitap Türü / Book Genre

- **Takas Talepleri Tablosu / Exchange Requests Table:**
  - Takas İsteyen Kullanıcı ID / User ID Requesting Exchange
  - Takas Edilecek Kitap ID / Book ID to be Exchanged
  - Takas Onay Durumu / Exchange Approval Status

- **Takas Geçmişi Tablosu / Exchange History Table:**
  - Gerçekleşen takasların geçmişi ve kullanıcıya özel takas önerileri için kullanılır.  
    Used for the history of completed exchanges and personalized exchange suggestions.

- **Geçici Token Tablosu / Temporary Token Table:**
  - Sunucu içindeki geçici token bilgilerini tutar.  
    Stores temporary token information within the server.

## Geliştirilmesi ve Eklenmesi Planlanan Özellikler / Features Planned for Development and Addition

- **Sohbet / Chat:** Kullanıcıların birbirleri ile sohbet edebileceği bir platform.  
  A platform where users can chat with each other.
- **Anlık Fotoğraf Çekme / Instant Photo Capture:** Kullanıcıların takas için kitap eklerken kameralarını kullanarak fotoğraf çekmeleri.  
  Allowing users to take photos with their cameras when adding a book for exchange.
- **Fotoğraftan Kitap Adı Tanıma / Book Title Recognition from Photo:** Yapay zeka kullanarak kitap adını fotoğraftan otomatik olarak tanıma.  
  Automatically recognizing the book title from the photo using artificial intelligence.
- **Takas Kitabı Önerisi / Exchange Book Suggestion:** Kullanıcının önceki takaslarına dayanarak yeni kitap önerileri sunma.  
  Offering new book suggestions based on the user's previous exchanges.

## Ekran Görüntüleri / Screenshots

![Screenshot 2024-06-21 022755](https://github.com/12enes34/savetree/assets/102800363/e35f00ee-da34-4e3e-9fe1-e55d0724f5f3)
![Screenshot 2024-06-21 022849](https://github.com/12enes34/savetree/assets/102800363/5b56e624-c161-4cb5-bc97-5788a6bf371d)
![Screenshot 2024-06-21 022945](https://github.com/12enes34/savetree/assets/102800363/9306c434-5424-4bc8-9903-94816fefa5ee)
![Screenshot 2024-06-21 023024](https://github.com/12enes34/savetree/assets/102800363/dbaa2425-8140-4b27-8cb0-ce2e24f600c9)

## Lisans / License

Bu proje MIT lisansı ile lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakın.  
This project is licensed under the MIT License. For more information, see the LICENSE file.
