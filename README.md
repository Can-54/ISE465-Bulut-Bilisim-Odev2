# ☁️ Bulut Bilişim Dersi Proje Ödevi

**Öğrenci:** Can Babaoğlu
**Durum:** ✅ Tamamlandı
**Canlı Bağlantı:** http://13.62.98.56

---

## 📌 Proje Özeti
Bu proje, **AWS EC2** bulut altyapısı kullanılarak statik bir web uygulamasının canlıya alınması (deployment) sürecini kapsar. Proje kapsamında sanal sunucu yönetimi, Linux komut satırı işlemleri ve ağ güvenliği (Security Groups) yapılandırmaları gerçekleştirilmiştir.

## 🛠 Kullanılan Teknolojiler
- **Bulut Sağlayıcı:** Amazon Web Services (AWS)
- **Sunucu:** EC2 (t3.micro) - Amazon Linux 2023
- **Web Servisi:** Apache HTTP Server
- **Arayüz:** HTML5 & CSS3

## 🏗 Uygulama Mimarisi

```mermaid
graph LR
    A[Kullanıcı] -- HTTP İstegi --> B((Internet))
    B -- Port 80 --> C{AWS Security Group}
    C -- İzin Verildi --> D[EC2 Sunucusu]
    D -- Apache Web Server --> E[index.html]
