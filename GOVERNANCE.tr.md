# Nexora proje yönetimi

[English](GOVERNANCE.md) · [Yol haritası](ROADMAP.tr.md) · [Marka](BRAND.tr.md)

Öncelikleri Nexora'nın sahibi belirler; kapsamı belli her çalışma paketini ayrıca onaylar. Katkı verenler ilgili deponun katkı rehberinden öneri sunabilir. Ürün sahipliği ve son yayın kararı sahibinde kalır.

## Karar süreci

1. **Öner:** kullanıcı sorununu, beklenen davranışı, etkilenen depoları, doğrulamayı, yayın hedefini ve varsa ücretli veya kalıcı işlemi açıkla.
2. **Onayla:** uygulamadan önce kapsamı kesinleştir. Paket onayı gerekli uygulama, düzeltme, test ve kararlaştırılan yayını kapsar; ilgisiz gelecek işleri yetkilendirmez.
3. **Tamamla:** kullanılabilir bir geliştirme bitir, farkları incele, değişikliğe uygun kontrolleri çalıştır ve yayımlanan sonucu doğrula. Kod değişikliklerinde PR ve commit'e bağlı CI kullan.
4. **Bildir:** bağlantıları, test kapsamını ve kalan sınırları paylaş. İnsan kabulü ile otomatik doğrulama ayrı kaydedilir. Başarısız veya ertelenmiş kontrol görünür kalır.

Yeni ürün, büyük mimari değişiklik ve kapsam genişlemesi yeniden önerilir. Harcama, depo silme, lisans değişikliği ve dış duyuru açık kapsam gerektirir. Bu belge otomatik bağımlılık birleştirmeyi veya zamanlanmış hesap yönetimini açmaz.

## Sürüm bütünlüğü

Etiketli kaynak, sürüm notu, sağlama toplamı ve paketler takip edilebilir kalsın. Mevcut sürümün kanıtı başka commit'in sonucuyla değiştirilmesin. Yalnızca belge güncellemesi çalışma sürümünü yükseltmeyi gerektirmez. Herkese açık demolar örnek veri kullanır ve sınırını belirtir.

Geçen testler değişikliğin incelenmesini sağlar; denenmemiş donanımda çeviri kalitesini, gerçek Discord davranışını veya FPS artışını kanıtlamaz. Bekleyen gerçek kullanım testleri ilgili ürünün doğrulama kaydında kalır.

## Erişim ve katkı

Anahtarlar, operatör bağlantıları, çalışma veritabanları, özel konuşmalar ve özel ticari kaynaklar açık paketlere girmez. Hesap ve barındırma erişimi onaylı işle sınırlı tutulur. Her ürünün lisansı ile model/bağımlılık bildirimleri ayrı geçerlidir.

Tekrar üretilebilir, hassas olmayan örnekler için hata formlarını; açıklar için etkilenen deponun `SECURITY.md` dosyasını kullan. Bir rapor herkese açık doğrulama hedefine sayılmadan önce bakımcı tarafından incelenir. Katılım gönüllüdür; kimlikler veya özel raporlar izinsiz yayımlanmaz.

## Güncel kapsam

Beta odağı VoiceBridge; diğer dört portföy ürünü bakımda. [Bağımlılık incelemesi](MAINTENANCE.tr.md) sekiz PR için işlem önerir; birleştirme onayı vermez. Gelecek uygulama paketleri ayrıca kararlaştırılır.
