# UI Requirement Map (Bab 2)

| ID | Requirement (Bab 1) | Halaman / Komponen | Field / Elemen | Alasan kebutuhan |
|----|---------------------|--------------------|----------------|------------------|
| FR-01 | Dashboard menampilkan ringkasan akademik | index.html | header, nav, section.dashboard-grid (3 card), aside.notice | Titik masuk aplikasi dan navigasi |
| FR-02 | Pengguna melihat profil mahasiswa | mahasiswa.html | figure+img, identitas (NIM, nama, email), tabel status akademik, tabel ringkasan | Menampilkan data mahasiswa |
| FR-03 | Pengguna mengisi data mahasiswa | form-mahasiswa.html | form: nim, nama, email, prodi, angkatan, status | Mengumpulkan data mahasiswa (disimpan ke DB pada Bab 6) |
| NFR-01 | Antarmuka valid, semantik, responsif | Semua halaman | doctype, lang, viewport, header/nav/main/footer | Aksesibilitas dan maintainability |
| NFR-02 | Tidak ada data sensitif di sisi client | Semua halaman | Data dummy, tanpa credential/token | Data minimization |

> Catatan: sesuaikan ID requirement dengan dokumen Bab 1 milik Anda.
