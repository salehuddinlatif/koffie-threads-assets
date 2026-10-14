# koffie-threads-assets

Aset gambar awam untuk auto-post **Threads @koffiejlnmentol** (Koffie Jln. Mentol, Segamat).

Meta cURL `image_url`, jadi URL mesti awam dan kekal. Repo ini menyimpan **gambar pemasaran sahaja**.

- `gallery/<slug>.jpg` — gambar kedai/minuman (JPEG, lebar 320–1440 px, ≤8 MB, nisbah aspek ≤10:1)
- `app/<slug>.jpg` — screenshot feature app KOFFIE (1170×2532 px)
- `manifest.json` — nama fail → URL raw + metadata + nisbah folder (`folders`)
  (dijana oleh `koffie_threads_media_build.py`)

Semua gambar post Threads datang dari repo ini (URL raw). Repo Pages `koffie-miniapp`
kekal untuk laman app sahaja — **jangan** guna URL `salehuddinlatif.github.io` sebagai `image_url`.

Jangan letak data bisnes, harga, token, atau apa-apa yang bukan gambar di sini — repo ini **awam**.

Jangan edit `manifest.json` dengan tangan. Jana semula (`--folder` memilih folder; entri folder
lain dalam manifest dikekalkan):

```
python %LOCALAPPDATA%\hermes\profiles\koffiecontent\scripts\threads\koffie_threads_media_build.py --apply --push
python %LOCALAPPDATA%\hermes\profiles\koffiecontent\scripts\threads\koffie_threads_media_build.py --folder app --source-dir %LOCALAPPDATA%\hermes\projects\koffie-content\screenshots-app --apply --push
```
