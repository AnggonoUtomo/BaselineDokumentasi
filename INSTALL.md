# Instalasi SEOS ke dalam Proyek

## Proyek Baru

Salin seluruh file dari paket SEOS ke root repository. Pertahankan `.gitignore` proyek yang sudah ada; gunakan `.gitignore.template-notes` hanya sebagai panduan.

Kemudian instruksikan AI:

```text
Baca AGENTS.md dan jalankan docs/00-governance/AI-PROJECT-BOOTSTRAP-PROMPT.md.
Jangan melakukan coding selama bootstrap. Periksa repository, pisahkan fakta terverifikasi dari asumsi, isi dokumen baseline sesuai urutan, dan akhiri dengan putusan kesiapan proyek.
```

## Proyek yang Sudah Berjalan

1. Salin `docs/`, `AGENTS.md`, dan `SEOS-VERSION`.
2. Gabungkan `README.md` dan instruksi agen secara hati-hati; jangan menimpa aturan proyek yang masih valid tanpa review.
3. Lakukan bootstrap berdasarkan bukti aktual di repository.
4. Daftarkan pekerjaan aktif dan keputusan arsitektur yang sudah diketahui.
5. Jangan mengarang bukti secara retrospektif untuk pekerjaan lama. Tandai informasi hasil rekonstruksi secara jelas.

## Memulai Work Item

```bash
cp -R docs/07-work-items/templates/<package> \
  docs/07-work-items/<collection>/<WORK-ID>-<slug>
```

Perbarui `WORK-ITEM-REGISTRY.md`, metadata, dan dokumen pra-pengerjaan sebelum coding dimulai.
