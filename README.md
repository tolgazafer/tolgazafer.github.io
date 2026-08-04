# tolgazaferozdemir.com

Tolga Zafer Özdemir'in kişisel sitesi. Canlı: <https://tolgazafer.github.io>

Site tek bir dosya: [`index.html`](index.html). CSS'i, JavaScript'i, 253 mektubun
verisi ve bütün metinler dosyanın içinde. Dışarıdan yalnızca `site/assets/`
altındaki medyayı çağırıyor — 251 görsel, 90 video, artı tünel görünümü için
tembel yüklenen `three.min.js`.

Jekyll çalıştırılmıyor (`.nojekyll`); GitHub Pages dosyaları olduğu gibi sunuyor.

## Bu klasör elle düzenlenmiyor

Üretilmiş bir kopyadır. Kaynağı ve içerik araçları private arşiv reposunda:
[tolgazafer/tolgazaferozdemir-arsiv](https://github.com/tolgazafer/tolgazaferozdemir-arsiv).
Orada proje kökünde:

```
python3 araclar/yayina-hazirla.py     # yayin/ klasörünü tazeler
cd yayin && git add -A && git commit && git push
```

Script sayfanın gerçekten referans verdiği medyayı kopyalar, gerekmeyeni siler.
`site/assets/...` yol öneki bilerek korunuyor: böylece yerel `file://` kopyası ile
yayındaki kopya bire bir aynı davranıyor, HTML'de hiçbir şey değiştirmek gerekmiyor.
