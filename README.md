
# 💬 Secomment
**Secomment**, statik web siteleri (Jekyll, Hugo, GitHub Pages) için geliştirilmiş, Firebase Realtime Database tabanlı, hafif ve modern bir yorum sistemidir.



## ✨ Özellikler
- 🚀 **Gerçek Zamanlı:** Yorumlar sayfa yenilenmeden anında iletilir ve görünür.
- 🛡️ **Onay Mekanizması:** Yorumlar önce admin paneline düşer, siz onaylamadan yayınlanmaz.
- 💬 **Yönetici Yanıtları:** Admin panelinden yorumlara özel yanıtlar verebilirsiniz.
- 🌙 **Karanlık Mod:** Cihaz temasına göre otomatik renk değiştirme.
- 📱 **Mobil Uyumlu:** Her türlü ekran boyutunda kusursuz görünüm.
- 🛠️ **Kolay Entegrasyon:** Tek bir `iframe` satırı ile her siteye uyumlu.

## 🚀 Hızlı Kurulum

### 1. Firebase Ayarları
1. [Firebase Console](https://console.firebase.google.com/) üzerinden bir proje oluşturun.
2. **Realtime Database**'i aktif edin.
3. **Rules** kısmına şu kuralları yapıştırın ve **Publish** butonuna basın:
   ```json
   {
     "rules": {
       ".read": true,
       ".write": true
     }
   }

 * Authentication kısmından e-posta/şifre girişini aktif edin ve kendiniz için bir admin hesabı oluşturun.
2. Dosyaları Düzenleyin
widcom.html ve admin.html dosyalarındaki const firebaseConfig kısmına kendi Firebase bilgilerinizi yapıştırın.
3. Sitenize Ekleyin
Yorumların görünmesini istediğiniz yere aşağıdaki kodu ekleyin:
<iframe 
  src="https://KULLANICI_ADINIZ.github.io/secomment/widcom.html?id=SAYFA_ID" 
  style="width: 100%; border: none; min-height: 500px;"
  allow="javascript">
</iframe>

🛠️ Teknolojiler
 * Altyapı: Firebase Realtime Database
 * Kimlik Doğrulama: Firebase Auth
 * Frontend: HTML5, CSS3 (Variables & Grid), JavaScript (ES6 Modules)
📄 Lisans
Bu proje MIT lisansı ile lisanslanmıştır.
Made with ❤️ by Sxinar

Projem TypeScript ve PocketBase veya Supabase ile güncellenecektir.
kişisel kullanım içindir.
