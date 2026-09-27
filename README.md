# latitudle-legal

[Latitudle](https://play.google.com/store/apps/details?id=com.afurkantitiz.latitudle)'ın
gizlilik politikasının yayımlandığı yer: <https://afurkantitiz.github.io/latitudle-legal/privacy.html>

**Bu repodaki HTML elle düzenlenmez.** Tek kaynak, uygulama reposundaki `docs/privacy.md`;
sayfa `tools/build_legal.py` ile ondan üretilir:

    python3 tools/build_legal.py     # bu repoya yazar
    git -C ../latitudle-legal commit -am "..." && git -C ../latitudle-legal push

Politika metni değişirse `docs/privacy.md`'yi düzenle ve komutu yeniden çalıştır. İki kopyayı
elle senkron tutmaya çalışmak, 1.14.1 denetiminde yakalanan hatanın ta kendisiydi: mağaza metni
ve gizlilik politikası, 1.6'da kaldırılmış bir renk paletini aylarca anlatmaya devam etmişti.

`outfit.ttf` sayfanın kendi fontu (OFL). Üçüncü taraf CDN'den çekilmiyor: "bu uygulama hiçbir
sunucuyla konuşmaz" diyen bir sayfanın font için başkasının sunucusuna gitmesi olmaz.
