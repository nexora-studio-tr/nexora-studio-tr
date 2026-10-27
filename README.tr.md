<p align="center">
  <img src="https://raw.githubusercontent.com/nexora-studio-tr/nexora-studio-tr/main/assets/header.webp" alt="Nexora" width="100%" />
</p>

[English](README.md) · [Türkçe](README.tr.md) · [Ürün yol haritası](ROADMAP.tr.md)

Diller arasında kaybolan bir konuşma, hatayı yakalayamayan bir test, süresi dolmasına rağmen açık kalan bir yetki: kolayca gözden kaçan sorunlar için açık kaynak araçlar geliştiriyorum.

Çalışmalarım **geliştirici araçları, Discord altyapısı ve performans ölçümü** üzerinde yoğunlaşıyor. Her projede Türkçe/İngilizce dokümantasyon, kurulum yönergeleri, otomatik testler ve açıkça belirtilmiş doğrulama sınırları bulunuyor.

## Seçili projeler

| Proje | Son sürümdeki anlamlı geliştirme | Sürüm |
| :--- | :--- | :--- |
| **[VoiceBridge](https://github.com/nexora-studio-tr/voicebridge)** | Discord için kişisel Türkçe ↔ İngilizce altyazı ve ses. Altyazı başına aşama süreleriyle kuyruk, tanıma ve çeviri gecikmesini inceleme. | [0.1.0-alpha.4](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.4) |
| **[ProofGate](https://github.com/nexora-studio-tr/proofgate)** | Kod değişikliği için test kanıtı ve bağımlılık gerekçeleriyle salt okunur workspace etki analizi. Test çalıştırma tek npm paketiyle sınırlı. | [0.1.0-alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2) |
| **[ReproPack](https://github.com/nexora-studio-tr/repropack)** | HTTP/PostgreSQL hatalarını küçültür; kalan adımların silme denemelerini ve kısmi kanıt durumunu açıklayan kayıtlar sunar. | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2) |
| **[AccessLease](https://github.com/nexora-studio-tr/accesslease)** | Bağımsız onaylı geçici Discord erişimi, doğrulanmış süre sonu ve beklerken ilk bitişi değiştirmeyen bağlantılı yenileme başvurusu. | [0.1.0-alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2) |
| **[Nexora FrameLab](https://github.com/nexora-studio-tr/nexora-framelab)** | Windows donanım algılama ve PresentMon kayıt karşılaştırması. Kalite kontrolleri, gözlenen farkı uyumsuz ölçümden ayırır. | [0.1.0-alpha.2 · Windows](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2) |

**Sürüm kapsamı:** bunlar doğrulama kayıtları ve SHA-256 dosyaları bulunan alpha sürümleridir. VoiceBridge bağımsız çok kullanıcılı beta geri bildirimi bekliyor; AccessLease'in canlı Discord kabul testi yapılmadı. FrameLab için canlı CS2 ölçümü veya kanıtlanmış FPS artışı yok. İçe aktarılan kayıt karşılaştırması ayar uygulayamaz.

Sentetik verilerle **[ProofGate demosunu](https://proofgate-demo.onrender.com/)** ve **[ReproPack demosunu](https://repropack-demo-4rq9.onrender.com/)** inceleyebilir veya ilgili sürümün kurulum yönergelerini izleyebilirsin.

## Geliştirme yaklaşımım

- **Kontrol kullanıcıda kalsın.** Kendi cihazında/sunucunda çalışan uygulamalar, belgelenmiş yapılandırma ve açık işleme tercihleri.
- **Sonuçlar incelenebilsin.** Kodun yanında mimari açıklamalar, güvenlik politikaları, anlamlı testler ve doğrulama kayıtları.
- **Geri dönüş tasarımın parçası olsun.** İlgili projelerde izin iptali, süreli erişim, tekrar üretilebilir hatalar ve geri alınabilir ayar değişiklikleri.

**Temel araçlar:** TypeScript · Python · Rust · PostgreSQL · React · Tauri

## Sonraki sürüme katkı ver

Güncel beta odağı VoiceBridge. İkinci bir kişiyle deneyip konuşma tanıma hatalarını, izin davranışını veya dinleme gecikmesini **[beta başlığında paylaş →](https://github.com/nexora-studio-tr/voicebridge/issues/1)**. Özel konuşmaları, anahtarları ve sunucu kimliklerini ekleme.

Diğer projelerde ilgili hata formlarını ve katkı rehberlerini kullanabilirsin. Güvenlik açıkları için etkilenen deponun `SECURITY.md` dosyasını izle.
