# quarterly-tax-legal

1099 Quarterly Tax Estimator uygulamasının **gizlilik politikası + destek**
sayfaları. GitHub Pages ile yayınlanıyor; `lumi-journal-legal` ile aynı desen.

Yayın adresi (Pages açıldıktan sonra):

- https://unverfirat.github.io/quarterly-tax-legal/ — tanıtım
- https://unverfirat.github.io/quarterly-tax-legal/privacy.html — **App Store
  Connect'e girilecek Privacy Policy URL'i**
- https://unverfirat.github.io/quarterly-tax-legal/support.html — **Support URL**

⚠️ **Erişilemeyen gizlilik URL'i = kesin ret.** Pages yayına aldıktan sonra
iki adresi de tarayıcıda aç ve gerçekten açıldığını gör.

## Bu adresler nereye yazılı

| Yer | Alan |
|---|---|
| `lib/legal.dart` | `Legal.privacyUrl`, `Legal.supportUrl` (paywall'daki bağlantılar) |
| App Store Connect | App Information → Privacy Policy URL, Support URL |
| Play Console | Store listing → Privacy policy |

## Gizlilik metni RevenueCat'e göre yazıldı

`privacy.html` içindeki **Purchases** bölümü, RevenueCat'in bağlı olduğu
duruma göre yazılmış durumda. Anahtarlar (`purchases_service.dart`) henüz boş,
yani bugün RevenueCat'e hiçbir şey gitmiyor — metin fazla açıklıyor, eksik
değil. Bilinçli tercih: eksik açıklamak ret sebebi, fazla açıklamak değil.
Uygulamayı RevenueCat'siz yayınlamaya karar verirsen o bölümü sadeleştir.

## İçerik nereden geliyor

Kaynak metinler uygulama deposunda: `store_assets/privacy_policy.md`.
Politikayı değiştirirsen İKİSİNİ birden güncelle, yoksa mağazada yazan ile
sitede yazan ayrışır.

Sayfalarda iddia edilen her şey kodda doğrulanmış olmalı — özellikle
"CSV export ücretsiz", "40 eyalet + DC kapsamda, Connecticut değil",
"Idaho ve Utah çeyreklik istemiyor" cümleleri. Bunlar değişirse sayfa da
değişmeli.

## Yerelde bakmak

```bash
python3 -m http.server 8080
# http://localhost:8080/privacy.html
```
