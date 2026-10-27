# Ürün ve geliştirme yol haritası

[English](ROADMAP.md) · [Profil](README.tr.md)

Güncelleme: 27 Ekim 2026. Beş kullanılabilir geliştirme sırayla tamamlandı. Aşağıdaki kapılar doğrulama ve mimari çalışmalarıdır; teslim tarihi veya performans vaadi içermez.

| Ürün                | Yayımlanan geliştirme                                                                                                                                                             | Sıradaki anlamlı kapı                                                                                                                                                             |
| :------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **VoiceBridge**     | [Alpha.4](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.4): kuyruk dahil altyazı aşama süreleri ve iki dilde açıklamalar.                             | Bağımsız kurulum; iki kişinin dil yönleri, çakışan konuşma, kişisel ses ve izin iptalini denemesi. Süreler mikrofon kaydını, Discord aktarımını ve tarayıcıda dinlemeyi kapsamaz. |
| **ProofGate**       | [Alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2): salt okunur workspace bağımlılık etki analizi.                                              | Monorepo test çalıştırmaya geçmeden paketlere bağlı yürütme/kanıt mimarisini inceleme. Güncel çalıştırma tek npm/Vitest paketiyle sınırlı.                                        |
| **ReproPack**       | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2): kalan adımların silme denemeleri ve açık kısmi kanıt durumu.                          | Registry yeniden başladığında korunan PostgreSQL tekrar durumu ve bağımsız pilot. Güncel snapshot ömrü registry ile sınırlı.                                                      |
| **AccessLease**     | [Alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2): ilk bitişi değiştirmeyen, başka kişinin onayını gerektiren bağlantılı yenileme başvurusu. | Özel Discord sunucusunda gerçek erişim, süre sonu, yönetici müdahalesi ve yeniden başlatma kabul testi. Bu test ertelenmiş durumda.                                               |
| **Nexora FrameLab** | [Alpha.2](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2): içe aktarılan kayıtlarda kalite kontrollü, gözleme dayalı karşılaştırma.              | FPS artışı veya iyileştirme iddiasından önce gerçek CS2 replay/kayıt/geri alma ve tanımlı donanım ölçümleri. Canlı oyun testi ertelenmiş durumda.                                 |

## Güncel odak ve sıra

1. **VoiceBridge: iki bağımsız temiz kurulum.** Gönüllülerin kurulum raporları incelenip kabul edilen kanıtlar [beta kaydına](https://github.com/nexora-studio-tr/voicebridge/blob/main/docs/BETA-STATUS.md) işlenecek. Yalnızca kayıtlı demoyu çalıştırmak yeterli sayılmaz. Henüz incelenmiş bağımsız kurulum sonucu iddia edilmiyor.
2. **VoiceBridge: aynı gerçek odada iki ayrı insan.** İki dil yönü, çakışan konuşma, kişisel ses ve izin iptali denenecek. Bu kapı kurulum başarısından ayrıdır. [Betaya katıl](https://github.com/nexora-studio-tr/voicebridge/issues/1).
3. **Bakım:** onaylanan iki Actions güncellemesi birleştirildi; ana dal CI bağlantıları [bağımlılık kaydında](MAINTENANCE.tr.md). Sıradaki öneri, eski tabanlı dört Actions dalını güncelleyip birleştirmeden önce güncel CI sonuçlarını doğrulamak. Node 26 tip yükseltmeleri birleştirilmeden bekliyor. Yeni değişiklikler ayrı onaylı paket gerektirir.

Geri bildirim toplanırken diğer dört ürünün odağı bakım. Yeni ürün kapsamları ve büyük mimari değişiklikler [yönetim rehberine](GOVERNANCE.tr.md) göre ayrıca kararlaştırılır.

Kurulum kontrolleri ve altyazı aşama süreleri teşhise yardımcı olur; konuşma kalitesini, uçtan uca dinleme gecikmesini veya kapasiteyi kanıtlamaz. Teslim tarihi, katılımcı sayısı veya yıldız artışı garantisi verilmez.

Her sürüm anlamlı otomatik kontroller, kaynak/sürüm kimliği, kurulum yönergeleri ve Türkçe/İngilizce belgeler içerir. Bağımsız insan kabulü ve ertelenen canlı testler ayrıca belirtilir. Tekrar üretilebilir kullanıcı geri bildirimleri sonraki geliştirme önceliğini belirler.
