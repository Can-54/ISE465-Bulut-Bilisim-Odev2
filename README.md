# ISE 465 - Bulut Bilişim Dersi 2. Ödev Raporu

**Öğrenci:** Can Babaoğlu
**Proje Durumu:** Başarıyla tamamlandı ve canlı yayında.
**Canlı Yayın Bağlantısı:** http://13.62.98.56

---

## 1. Proje Açıklaması ve Hedefleri

Bu projenin temel hedefi, bulut bilişim kavramlarını anlamak ve IaaS (Infrastructure as a Service) modeli üzerinde çalışan basit bir web uygulamasının dağıtımını gerçekleştirmektir. Proje kapsamında, sektör standardı olan bir bulut sağlayıcısı (AWS) kullanılarak, temel düzeyde altyapı yönetimi becerileri geliştirilmiştir.

## 2. Uygulama Seçimi ve Bulut Platformunun Seçilmesi

* **Uygulama Seçimi:** Statik bir web sayfası yayınlayan basit bir web uygulamasıdır.
* **Platform Seçimi:** Amazon Web Services (AWS) tercih edilmiştir. Platform, yaygın kaynakları ve ücretsiz kullanım (Free Tier) imkanları nedeniyle seçilmiştir.
* **Kullanılan Servisler:** EC2 (Sanal Makine), Security Group (Güvenlik Duvarı), Amazon Linux 2023.
* **Kaynak Silme Uyarısı:** Proje ödevi bittiğinde ücretlendirme ile karşılaşmamak için ilgili kaynaklar silinecektir.

## 3. Uygulama Mimarisi Şeması (Basitleştirilmiş)

```mermaid
graph TD
    A[Kullanıcı/Öğrenci] --> B(İnternet);
    B --> C(AWS Sanal Ağ Kapısı / Security Group);
    C --> D(EC2 Sanal Makinesi);
    D --> E(Apache HTTP Sunucusu);
    E --> F(HTML Web Sayfası);
