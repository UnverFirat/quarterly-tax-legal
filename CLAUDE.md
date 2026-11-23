# CLAUDE.md — quarterly-tax-legal

Bu dosya, bu projede çalışan Claude Code için kalıcı talimatlardır. Proje ayrıntıları için README.md ve STATUS.md'ye bak.

## Durum takibi (apptracker)
Bu repo `~/IdeaProjects/apptracker.py` panosunda izleniyor. Pano repo kökündeki `STATUS.md`'yi okur.

**Ne zaman:** Her çalışma oturumunun sonunda, commit atmadan hemen önce ve kullanıcı "durumu güncelle" dediğinde.

**Nasıl:**
- `STATUS.md`'yi aşağıdaki formatta güncelle; dosya yoksa oluştur.
- Mevcut içeriği silme: biten görevi `- [x]` yap, yeni çıkan işi `- [ ]` olarak "Sıradaki"ye ekle, "Nerede kaldık"ı o anki duruma göre yeniden yaz.
- `özet:` tek satır, en fazla ~120 karakter; yalnızca şu anki durum ve sıradaki adım.
- `güncelleme:` bugünün tarihi (YYYY-MM-DD).
- `STATUS.md` değişikliğini işle aynı commit'e koy.

```
durum: <canlı | geliştirme | fikir | destek | durduruldu>
özet: <tek cümle: şu an nerede olduğumuz>
güncelleme: <YYYY-MM-DD>
---
## Nerede kaldık
<2-5 cümle: son yapılan iş, yarım kalan şey, hangi dosyalarda, aktif dal>
## Sıradaki
- [ ] <somut, tek oturumda bitebilecek görev>
## Bitenler
- [x] <tamamlanan görev>
## Engeller / notlar
- <store review, bekleyen karar, bilinen bug vb.>
```
