# Kablolama Asistanı — Güncelleme Deposu

Bu depo **sadece kurulum dosyalarını** dağıtır (kaynak kod burada değildir).

Kurulu programlar AutoCAD açıldıktan ~20 sn sonra şu adrese bakar:

```
https://github.com/eymennegeeokurr-rgb/kablolama-guncelleme/releases/latest/download/surum.txt
```

Yeni sürüm varsa `KablolamaAsistani_Setup.exe` arka planda indirilir ve
AutoCAD kapatılınca sessizce kurulur.

## Yeni sürüm yayınlama

1. Visual Studio'da derleyin, `Kurulum\PaketOlustur.bat`'a çift tıklayın.
2. Bilgisayarda **GitHub CLI** (`gh`) kurulu ve `gh auth login` yapılmışsa yükleme kendiliğinden olur.
3. Değilse açılan **Releases → New release** sayfasında:
   - Tag: `v<sürüm>` (pencerede yazar)
   - `Kurulum\Yayin` klasöründeki **iki dosyayı** sürükleyin: `KablolamaAsistani_Setup.exe` ve `surum.txt`
   - **Publish release**

Her zaman *en son* yayın kullanılır; eski yayınları silmeye gerek yoktur.
