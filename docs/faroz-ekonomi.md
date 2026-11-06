# Faroz · Sürüm 2 ekonomi tablosu

Bütün değerler `faroz.html` içindeki `CFG` bloğundadır. Süreler, oyunu hedef karelere ışınlanarak oynayan test botuyla (390×844, `window.__faroz.update`) ölçüldü. Gerçek oyuncu yürüdüğü için yaklaşık 1,5–2 kat uzun sürer.

## Fiyatlar (tezgâh / market, birim)

| Ürün | Taban | Bölüm 1 (×1) | Bölüm 2 (×1,3) | Bölüm 3 (×1,7) | Mühürlü (×1,5) |
|---|---|---|---|---|---|
| Hamsi | 3 | 3 | 4 | 5 | — |
| Temiz hamsi | 7 | 7 | 9 | 12 | 11 |
| Tuzlu hamsi | 13 | 13 | 17 | 22 | 20 |
| Tütsülü hamsi | 24 | 24 | 31 | 41 | 36 |
| Yaş çay | 4 | — | 5 | 7 | — |
| Kuru çay (2 yaş çay) | 30 | — | 39 | 51 | 59 |
| Fındık | 5 | — | — | 9 | — |
| Kavrulmuş fındık (2 fındık) | 34 | — | — | 58 | 87 |

Bölüm 4 (yayla sezonu, ×2,2):

| Ürün | Taban | Bölüm 4 | Mühürlü |
|---|---|---|---|
| Süt | 6 | 13 | — |
| Yayla peyniri (2 süt) | 44 | 97 | 145 |
| Petek | 10 | 22 | — |
| Yayla balı (2 petek) | 40 | 88 | 132 |

**Koli (Bölüm 3, kamyon):** 5 birim × taban × 2,0 (toptan) × 1,7 (dönem) × (1 + ün/400). Ün 100'deyken bir koli tütsülü ≈ 510 ₺, koli çay ≈ 640 ₺, koli kavrulmuş ≈ 720 ₺. Mühürlü koli ×1,3. Sözleşme tamamlanınca yüklenenin %25'i kadar bahşiş gelir.

**Gerekçe:**
- İşleme belirgin kârlı. 2 yaş çay (10 ₺) → 1 kuru çay (39 ₺); 2 fındık → kavrulmuş, 7 kat değer.
- Testte çiğ çay 43, kuru çay 504 adet satıldı. Ege'deki "çoğu çiğ satıldı" sorunu tekrarlanmadı.
- Kasabada aynı mal koliyle tezgâhtaki fiyatının 2 katına gider. "Toptan daha iyi öder" kuralı fiyatla hissediliyor, ekranda ek gösterge yok.

## Alan ve bina maliyetleri

| Bölüm | Alan | ₺ | Not |
|---|---|---|---|
| 1 | Ayıklama · Küfe · Nazmiye · Tuzlama | 30 · 60 · 90 · 150 | |
| 1 | Temel · Fadime · Tütsühane · Hamdi · İdris · Büyük küfe | 220 · 280 · 380 · 420 · 520 · 300 | |
| 1 | **Kapı:** dakikada 480 ₺ | — | hamsi zinciri kendi dönüyor mu |
| 1 | Yalı evi | 1.200 + 3 mühürlü tütsülü | bölüm sonu |
| 2 | Çay bahçesi · Fabrika · Köy evi · Zehra | 600 · 1.200 · 1.800 · 2.200 | |
| 2 | İkinci teras · Kazım · İkinci tütsü ocağı · Köy evi | 2.800 · 3.200 · 2.600 · 3.800 | ikinci ocak, ölçülen darboğazı açar |
| 2 | **Kapı:** dakikada 1.800 ₺ | — | çay da kendi dönüyor mu |
| 2 | Çay ocağı | 6.000 + 4 mühürlü kuru çay | bölüm sonu |
| 3 | Rampa · Pakethane · Fındık · Kavurma | 5.000 · 6.500 · 7.500 · 9.000 | |
| 3 | Hüsnü · İkinci tekne · Market · Cafer | 9.500 · 8.000 · 12.000 · 12.000 | |
| 3 | **Kapı:** 4 sözleşme ve dakikada 6.000 ₺ | — | |
| 3 | Hamsi Festivali | 30.000 + 2 mühürlü koli tütsülü | bölüm sonu |
| 4 | Yayla yolu · Ahır · Mandıra · Murat | 15.000 · 18.000 · 22.000 · 24.000 | |
| 4 | Kovanlar · Bal süzme · Dursun · Yayla evi | 26.000 · 28.000 · 30.000 · 32.000 | |
| 4 | **Kapı:** dakikada 14.000 ₺ | — | yayla da kendi dönüyor mu |
| 4 | Yayla şenliği | 60.000 + 4 mühürlü peynir | bölüm sonu, dayının sırrı açılır |

**Hedef:** Her alanın bedeli, o dönemdeki dakikalık kazancın 1–3 katı olsun.

## Ölçülen dakikalık kazanç (bot)

| An | ₺/dk | Bölüm süresi (bot) |
|---|---|---|
| Bölüm 1 başı → sonu | 15 → ~650–980 | 8,2 dk |
| Bölüm 2 başı → sonu | ~650 → ~2.000–3.000 | 12,1 dk |
| Bölüm 3 başı → sonu | ~2.300 → ~8.000–9.700 | 17,5 dk |
| Bölüm 4 başı → sonu | ~3.000 → ~17.000–24.000 | 18,6 dk |

Oyuncu hiçbir şey yapmadan 2 dakika bekletilerek ölçülen otomatik üretim ve satış:

| Bölüm sonu | Kazanç (₺/dk) | Satılan (adet/dk) | Ün |
|---|---|---|---|
| 1 | 647 | tütsülü 24,5 · tuzlu 4,5 | 85 |
| 2 | 2.078 | tütsülü 42,5 · kuru çay 19,5 | 100 |
| 3 | 7.942 | kavrulmuş 17 · tütsülü 11,5; fazlası kamyona | 100 |

Maaş yok. Faroz'da çalışan bir kez işe alınır, gider kalemi taşımaz. Bu yüzden Ege'deki "kasa 3 ₺'yle bitti" sorunu burada oluşmaz.
