<p align="center">
  <img src="https://raw.githubusercontent.com/nexora-studio-tr/nexora-studio-tr/main/assets/header.webp" alt="Nexora" width="100%" />
</p>

[English](README.md) · [Türkçe](README.tr.md) · [Ürün yol haritası](ROADMAP.tr.md)

Diller arasında kaybolan bir konuşma, hatayı yakalayamayan bir test, süresi dolmasına rağmen açık kalan bir yetki: kolayca gözden kaçan sorunlar için açık kaynak araçlar geliştiriyorum.

Çalışmalarım **geliştirici araçları, Discord altyapısı ve performans ölçümü** üzerinde yoğunlaşıyor. Her projede Türkçe/İngilizce dokümantasyon, kurulum yönergeleri ve açıkça belirtilmiş doğrulama sınırları bulunuyor.

## Seçili projeler

| Proje | Çözdüğü sorun | Başlangıç |
| :--- | :--- | :--- |
| **[VoiceBridge](https://github.com/nexora-studio-tr/voicebridge)** | Discord için kişiye özel Türkçe ↔ İngilizce altyazı ve ses. Yerel modeller, konuşmacı izni ve kişisel dinleme. | [alpha.3 / beta](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.3) |
| **[ProofGate](https://github.com/nexora-studio-tr/proofgate)** | Testin kod değişikliğini hatalı önceki sürümden ayırt edip etmediğini kontrol eder. Sınırlı mutasyon kanıtı, CLI ve MCP sunar. | [Salt okunur demo](https://proofgate-demo.onrender.com/) |
| **[ReproPack](https://github.com/nexora-studio-tr/repropack)** | HTTP/PostgreSQL hata senaryolarını, aynı hata imzasını koruyan daha küçük ve doğrulanmış örneklere indirger. | [Etkileşimli demo](https://repropack-demo-4rq9.onrender.com/) |
| **[AccessLease](https://github.com/nexora-studio-tr/accesslease)** | Geçici Discord erişimine bağımsız onay, izin önizlemesi ve doğrulanmış süre sonu ekler. | [alpha.1 / kurulum](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.1) |
| **[Nexora FrameLab](https://github.com/nexora-studio-tr/nexora-framelab)** | Windows donanımını algılar, CS2 kare sürelerini analiz eder ve geri alınabilir ayar deneylerini değerlendirir. | [Deneysel Windows alpha](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.1) |

**Sürüm kapsamı:** projeler erken aşamadadır. VoiceBridge çok kullanıcılı beta geri bildirimi bekliyor; AccessLease'in canlı Discord kabul testi henüz yapılmadı. FrameLab için canlı CS2 ölçümü veya kanıtlanmış FPS artışı yok. Demo verileri ve çalışma sınırları ilgili depolarda belirtiliyor.

## Geliştirme yaklaşımım

- **Kontrol kullanıcıda kalsın.** Kendi cihazında/sunucunda çalışan uygulamalar, belgelenmiş yapılandırma ve açık işleme tercihleri.
- **Sonuçlar incelenebilsin.** Kodun yanında mimari açıklamalar, güvenlik politikaları, anlamlı testler ve doğrulama kayıtları.
- **Geri dönüş tasarımın parçası olsun.** İlgili projelerde izin iptali, süreli erişim, tekrar üretilebilir hatalar ve geri alınabilir ayar değişiklikleri.

**Temel araçlar:** TypeScript · Python · Rust · PostgreSQL · React · Tauri

## Sonraki sürüme katkı ver

Güncel beta odağı VoiceBridge. İkinci bir kişiyle deneyip konuşma tanıma hatalarını, izin davranışını veya dinleme gecikmesini **[beta başlığında paylaş →](https://github.com/nexora-studio-tr/voicebridge/issues/1)**. Özel konuşmaları, anahtarları ve sunucu kimliklerini ekleme.

Diğer projelerde ilgili hata formlarını ve katkı rehberlerini kullanabilirsin. Güvenlik açıkları için etkilenen deponun `SECURITY.md` dosyasını izle.
