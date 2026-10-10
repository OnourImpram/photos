# @kecipsikologu — Instagram yayın arşivi

Bu depo, [@kecipsikologu](https://www.instagram.com/kecipsikologu/) hesabı için **yayına hazırlanmış ve onaylanmış görsel içerikleri** ve bunların yayın metinlerini sürümlü olarak saklar.

## Düzen

```text
photos/
├── README.md
├── brand/
│   ├── DESIGN.md             # Görsel kimlik ve üretim kuralları
│   └── WRITING.md            # Türkçe editoryal üslup
└── posts/
    └── YYYY-MM-DD-kisa-baslik/
        ├── caption.md        # Instagram açıklaması
        ├── metadata.json     # Tarih, kanal, medya sırası, alternatif metin
        └── slides/
            ├── 01.png
            └── ...
```

## Yayın işleyişi

1. Metin ve tasarım kontrol edilip onaylanır.
2. Paylaşılabilir PNG/JPG dosyaları bu **Public** repoya yüklenir; URL'ler tek tek test edilir.
3. Buffer üzerinden Instagram Business hesabına otomatik yayın planlanır; sıra, saat, görsel sayısı ve durum doğrulanır.
4. Yayınlanacak bir gönderinin görsel URL'leri **yayın tamamlanana kadar** değiştirilmez, silinmez veya yeniden adlandırılmaz.
5. İçerik güncellemeleri sürüm kontrolüyle takip edilir. Alt metinler erişilebilirlik için korunur.

**Dikkat:** Bu repo herkese açıktır. Danışan bilgileri, sağlık verileri, gizli yazışmalar, ekonomik hedefleme stratejileri, kurum içi analizler, API anahtarları, henüz onaylanmamış özel materyaller ve kişisel bilgiler buraya yüklenmez.

Kullanılan görseller ve metinler, ayrıca belirtilmedikçe **© Onour Impram — Tüm hakları saklıdır.** Depoya herkese açık erişim verilmesi içerikleri yeniden kullanma izni anlamına gelmez.

Sorumlu hesap: [@kecipsikologu](https://www.instagram.com/kecipsikologu/) · Proje başlangıcı: Ekim 2026.

## İlk onaylı gönderi

- [13.10.2026 — Takviminiz dolu. Peki, hayatınız kimin?](posts/2026-10-13-takviminiz-dolu/)
- Instagram için kaynak dosyalar 7 PNG (1080 × 1350); caption ve yayın metadatası aynı klasördedir.
- Planlı yayın için Buffer sabit bir Git commit’ine işaret eder; yeni bir tasarım revizyonu eski URL’yi bozmaz.
- `validate-assets.yml` her yayın arşivi değişikliğinde medya sırasını ve görsel ölçülerini denetler.
