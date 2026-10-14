# koffie-threads-assets

Aset gambar awam untuk auto-post **Threads @koffiejlnmentol** (Koffie Jln. Mentol, Segamat).

Meta cURL `image_url`, jadi URL mesti awam dan kekal. Repo ini menyimpan **gambar pemasaran sahaja**.

- `gallery/<slug>.jpg` — gambar (JPEG, lebar 320–1440 px, ≤8 MB, nisbah aspek ≤10:1)
- `manifest.json` — nama fail → URL raw + metadata (dijana oleh `koffie_threads_media_build.py`)

Jangan letak data bisnes, token, atau apa-apa yang bukan gambar di sini — repo ini **awam**.

Jangan edit `manifest.json` dengan tangan. Jana semula:

```
python %LOCALAPPDATA%\hermes\profiles\koffiecontent\scripts\threads\koffie_threads_media_build.py --apply --push
```
