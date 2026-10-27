# Ürün ve geliştirme yol haritası

[English](ROADMAP.md) · [Profil](README.tr.md)

Güncelleme: 27 Ekim 2026. Bu liste geliştirme sırasıdır; teslim tarihi veya performans vaadi değildir. Bir kullanılabilir geliştirme dilimi tamamlanınca sonraki uygulamaya geçilir.

| Öncelik | Ürün | Sonraki anlamlı sonuç |
| :--- | :--- | :--- |
| **Güncel geliştirme** | **VoiceBridge** | [Alpha.3](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.3): yönlendirmeli kurulum kontrolü ve kullanıcı incelemesiyle indirilen özel destek raporu. [Uygulama ve kontroller](https://github.com/nexora-studio-tr/voicebridge/pull/2). |
| **Sıradaki mimari** | **ProofGate** | npm monorepolarında paket/bağımlılık grafiğini sabitleyen, etkilenen testleri seçen ve önce/sonra kanıtını paketlere bağlayan doğrulama tasarımı. Güncel destek tek npm paketiyle sınırlıdır. |
| **Sonraki araştırma** | **ReproPack** | PostgreSQL hata tekrarlama durumunu yeniden başlatmalar arasında koruyan tasarım. Güncel snapshot'lar çalışan kayıt sisteminin ömrüyle sınırlıdır; başarılı demo kalıcı tekrar kanıtı değildir. |
| **Kabul testi bekliyor** | **AccessLease** | Özel test sunucusunda gerçek erişim verme, süre sonu, dışarıdan rol değişikliği ve yeniden başlatmadan toparlanmayı sınama. Canlı kabul testi ertelenmiş durumdadır. |
| **Deneysel** | **Nexora FrameLab** | İyileştirme veya FPS artışı iddiasından önce gerçek CS2 tekrar/kayıt/geri alma akışını doğrulayıp tanımlı donanımlarda sonuç toplama. Canlı oyun testi ertelenmiş durumdadır. |

## Kullanıcı doğrulamasında sıradaki kapı

VoiceBridge için başka bir insanın bağımsız kurulumu ve iki ayrı kişinin iki çeviri yönünü, çakışan konuşmayı, kişisel sesi ve izin iptalini denemesi gerekiyor. Kurulum kontrolü bir durum görüntüsüdür; konuşma kalitesi veya gerçek test kanıtı değildir. [Betaya katıl](https://github.com/nexora-studio-tr/voicebridge/issues/1).

Her geliştirme; anlamlı testler, tekrarlanabilir kurulum, kaynak/sürüm kimliği ve Türkçe/İngilizce yönergelerle ilerler. Bir sonraki büyük genişletmenin mimarisi uygulamadan önce incelenir. Gerçek geri bildirimler ve tekrar üretilebilen hatalar bu sırayı değiştirebilir.
