# Ürün ve geliştirme yol haritası

[English](ROADMAP.md) · [Profil](README.tr.md)

Güncelleme: 27 Ekim 2026. Beş kullanılabilir geliştirme sırayla tamamlandı. Aşağıdaki kapılar doğrulama ve mimari çalışmalarıdır; teslim tarihi veya performans vaadi içermez.

| Ürün | Yayımlanan geliştirme | Sıradaki anlamlı kapı |
| :--- | :--- | :--- |
| **VoiceBridge** | [Alpha.4](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.4): kuyruk dahil altyazı aşama süreleri ve iki dilde açıklamalar. | Bağımsız kurulum; iki kişinin dil yönleri, çakışan konuşma, kişisel ses ve izin iptalini denemesi. Süreler mikrofon kaydını, Discord aktarımını ve tarayıcıda dinlemeyi kapsamaz. |
| **ProofGate** | [Alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2): salt okunur workspace bağımlılık etki analizi. | Monorepo test çalıştırmaya geçmeden paketlere bağlı yürütme/kanıt mimarisini inceleme. Güncel çalıştırma tek npm/Vitest paketiyle sınırlı. |
| **ReproPack** | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2): kalan adımların silme denemeleri ve açık kısmi kanıt durumu. | Registry yeniden başladığında korunan PostgreSQL tekrar durumu ve bağımsız pilot. Güncel snapshot ömrü registry ile sınırlı. |
| **AccessLease** | [Alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2): ilk bitişi değiştirmeyen, başka kişinin onayını gerektiren bağlantılı yenileme başvurusu. | Özel Discord sunucusunda gerçek erişim, süre sonu, yönetici müdahalesi ve yeniden başlatma kabul testi. Bu test ertelenmiş durumda. |
| **Nexora FrameLab** | [Alpha.2](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2): içe aktarılan kayıtlarda kalite kontrollü, gözleme dayalı karşılaştırma. | FPS artışı veya iyileştirme iddiasından önce gerçek CS2 replay/kayıt/geri alma ve tanımlı donanım ölçümleri. Canlı oyun testi ertelenmiş durumda. |

## Kullanıcı doğrulamasında sıradaki kapı

Beta odağı VoiceBridge. İki ayrı kişi iki dil yönünü, çakışan konuşmayı, kişisel sesi ve izin iptalini denemeli. Kurulum kontrolleri ve altyazı aşama süreleri teşhise yardımcı olur; konuşma kalitesini, uçtan uca dinleme gecikmesini veya kapasiteyi kanıtlamaz. [Betaya katıl](https://github.com/nexora-studio-tr/voicebridge/issues/1).

Her sürüm anlamlı otomatik kontroller, kaynak/sürüm kimliği, kurulum yönergeleri ve Türkçe/İngilizce belgeler içerir. Bağımsız insan kabulü ve ertelenen canlı testler ayrıca belirtilir. Tekrar üretilebilir kullanıcı geri bildirimleri sonraki geliştirme önceliğini belirler.
