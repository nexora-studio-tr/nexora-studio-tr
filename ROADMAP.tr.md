# Ürün ve geliştirme yol haritası

[English](ROADMAP.md) · [Profil](README.tr.md)

Güncelleme: 29 Ekim 2026. Beş ürünün etiketli alpha sürümü var. Güncel kalite ve beta odağı VoiceBridge; sonraki büyük geliştirme ProofGate. Aynı anda tek büyük özellik paketi yürütülür.

| Ürün                | Yayımlanan geliştirme                                                                                                                                                                     | Sıradaki anlamlı kapı                                                                                                                             |
| :------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------ |
| **VoiceBridge**     | [Alpha.7](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.7): operatör performans görünümü, özel sayısal raporlar, güvenli oda kurtarma ve Windows başlatıcısı. | Tekrarlanabilir TR/EN kalite başlangıcı; sonra kanıta göre iyileştirme. Bağımsız kurulum ve kullanıcının canlı kabulü ayrı kaydedilir.            |
| **ProofGate**       | [Alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2): salt okunur workspace bağımlılık etki analizi.                                                      | Monorepo test çalıştırmaya geçmeden paketlere bağlı yürütme/kanıt mimarisini inceleme. Güncel çalıştırma tek npm/Vitest paketiyle sınırlı.        |
| **ReproPack**       | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2): kalan adımların silme denemeleri ve açık kısmi kanıt durumu.                                  | Registry yeniden başladığında korunan PostgreSQL tekrar durumu ve bağımsız pilot. Güncel snapshot ömrü registry ile sınırlı.                      |
| **AccessLease**     | [Alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2): ilk bitişi değiştirmeyen, başka kişinin onayını gerektiren bağlantılı yenileme başvurusu.         | Özel Discord sunucusunda gerçek erişim, süre sonu, yönetici müdahalesi ve yeniden başlatma kabul testi. Bu test ertelenmiş durumda.               |
| **Nexora FrameLab** | [Alpha.2](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2): içe aktarılan kayıtlarda kalite kontrollü, gözleme dayalı karşılaştırma.                      | FPS artışı veya iyileştirme iddiasından önce gerçek CS2 replay/kayıt/geri alma ve tanımlı donanım ölçümleri. Canlı oyun testi ertelenmiş durumda. |

## Güncel odak ve sıra

1. **VoiceBridge: kalite başlangıcını ölç.** Kaynak/model kimlikleri belgelenmiş 30 Türkçe ve 30 İngilizce referans cümlesini karşılaştır. Sentetik örnekleri işaretle; tanıma hatalarını ve kritik çeviri anlam hatalarını ayrı raporla. Önce ölç, sonra değişiklik gerekip gerekmediğine karar ver. Bu başlangıç çalışması plan; yayımlanmış sonuç değil.
2. **VoiceBridge: bağımsız kurulum geri bildirimi.** Temiz tam sunucu kurulum raporlarını [beta kaydında](https://github.com/nexora-studio-tr/voicebridge/blob/main/docs/BETA-STATUS.md) incele. İlk öğrenme hedefi iki gönüllü; henüz incelenmiş bağımsız kurulum sonucu iddia edilmiyor. Yalnızca kayıtlı demo yeterli sayılmaz. [Betaya katıl](https://github.com/nexora-studio-tr/voicebridge/issues/1).
3. **ProofGate: workspace çalıştırmadan önce mimari.** Kaynak, paket, politika ve kanıt kimliğine bağlı dar npm-workspace/Vitest yolunu tasarla. Kapsam incelemesinden sonra uygula. Güncel çalıştırma tek paketle sınırlı.
4. **Bakım:** onaylanan altı Actions güncellemesinin tamamı birleştirildi; başarılı ana dal CI bağlantıları [bağımlılık kaydında](MAINTENANCE.tr.md). Windows Node yama seçimi ve tekrarlanan CI işleri de kayıtlı. İki Node 26 tip yükseltmesi birleştirilmeden bekliyor; çalışma sürümü/tip desteği değişikliği ayrı onaylı paket gerektirir.

VoiceBridge paketi sürerken diğer dört ürünün odağı bakım. Canlı Discord testleri kullanıcıda ve geliştirmeyi veya mimari çalışmayı bekletmez. İki dil yönü, çakışan konuşma, kişisel ses ve izin iptali için iki kişilik kabul hâlâ ayrı gerekiyor. Yeni ürün kapsamları ve büyük mimari değişiklikler [yönetim rehberine](GOVERNANCE.tr.md) göre ayrıca kararlaştırılır.

Kurulum kontrolleri ve altyazı aşama süreleri teşhise yardımcı olur; konuşma kalitesini, uçtan uca dinleme gecikmesini veya kapasiteyi kanıtlamaz. Teslim tarihi, katılımcı sayısı veya yıldız artışı garantisi verilmez.

Her sürüm anlamlı otomatik kontroller, kaynak/sürüm kimliği, kurulum yönergeleri ve Türkçe/İngilizce belgeler içerir. Bağımsız insan kabulü ve ertelenen canlı testler ayrıca belirtilir. Tekrar üretilebilir kullanıcı geri bildirimleri sonraki geliştirme önceliğini belirler.
