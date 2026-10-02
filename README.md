# Kafe — Örnek Web Tasarımları

Butik kafe ve restoranlara gösterilmek üzere hazırlanmış örnek web sitesi tasarımları.
Görüşmelerde "böyle bir şey yapıyoruz" diye göstermek için kullanılır.

## Şablonlar

| Klasör | Tarz | Esin kaynağı |
| --- | --- | --- |
| `01-zarif` | Koyu zemin, altın vurgu, el yazısı başlıklar, üst duyuru şeridi | Klasik restoran teması |
| `02-sicak` | Kahve rengi üst menü, yuvarlak rozet, krem vurgu kutuları, turuncu düğmeler | Kahve dükkânı teması |
| `03-sade` | Tam ekran fotoğraf, ince ve geniş aralıklı başlık, beyaz hap düğme | Modern minimal restoran |

`index.html` üçünü listeleyen seçim sayfasıdır; görüşmede önce bunu açıp aralarında gezinebilirsiniz.

## Açma

Derleme gerekmez. Kökteki `index.html` dosyasını çift tıklamak yeterli.
İnternet bağlantısı gerekmez: yazı tipi, görsel ya da betik dışarıdan çekilmez.

Yerel sunucuyla bakmak isterseniz (her tasarım ayrı portta):

```bash
npx serve -l 4201 .
npx serve -l 4202 .
npx serve -l 4203 .
```

- http://localhost:4201/01-zarif/
- http://localhost:4202/02-sicak/
- http://localhost:4203/03-sade/

## Fotoğraflar

Tüm şablonlar kökteki ortak `gorseller/` klasörünü kullanır (`../gorseller/...`).
Fotoğraflar Unsplash'ten alınmıştır; lisansı ticari kullanıma ve değiştirmeye izin verir,
atıf zorunlu değildir. İşletmenin kendi fotoğrafları geldiğinde bu dosyaların üzerine aynı
isimle yazmak yeterli, CSS'e dokunmaya gerek kalmaz.

| Dosya | Kullanıldığı yer |
| --- | --- |
| `hero-yemek.jpg` · `kahve-1.jpg` · `hero-masa.jpg` | Üç tasarımın kahraman alanları |
| `yemek-1..3.jpg` | Menü ve galeri kartları |
| `kahve-1..3.jpg` | Kahve ürün kartları |
| `mekan-1..3.jpg` | Galeri ve mekân görselleri |

## Notlar

- **Üçü de deneme tasarımıdır**; hiçbir işletmenin adı, menüsü ya da fiyatı geçmez.
  İşletme adı yerine "Kafe Adı" / "Kahve Dükkânı", fiyat yerine "—" yazar.
- Telefon, e-posta ve adres alanları yer tutucudur (`0000 000 00 00`, `ornek@ornek.com`).
- `01-zarif` tasarımında rezervasyon formu yoktur; rezervasyon telefonla alınır.
- Formlar (bülten, rezervasyon) hiçbir yere bağlı değildir, gönderince uyarı verir.

## Yeni şablon eklemek

Yeni bir klasör açıp içine `index.html` ve `style.css` koymak yeterli; sonra kökteki
`index.html` içindeki kart ızgarasına bir bağlantı eklenir.
