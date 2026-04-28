# Portofolio mii.R

Website portofolio ini bisa di-deploy cepat ke GitHub Pages.

## Cara Deploy ke GitHub Pages

1. Buat repositori baru di GitHub.
   - Buka https://github.com/new
   - Isi nama repositori, misalnya `portofolio_lengkap`
   - Pilih `Public`
   - Jangan centang `Initialize this repository with a README` jika kamu akan menggunakan repo lokal.

2. Di folder lokal kamu, buka PowerShell lalu jalankan:

```powershell
cd "c:\Users\yulis\Downloads\portomiii\portofolio_lengkap"
git init
git add .
git commit -m "Initial commit"
```

3. Hubungkan repo lokal ke GitHub (ganti URL dengan repo kamu):

```powershell
git remote add origin https://github.com/<username>/<repo-name>.git
git branch -M main
git push -u origin main
```

4. Aktifkan GitHub Pages:
   - Buka repo GitHub kamu.
   - Masuk ke `Settings` > `Pages`.
   - Pada `Source`, pilih `main` branch dan folder `/ (root)`.
   - Klik `Save`.

5. Setelah beberapa saat, GitHub akan memberi URL seperti:
   `https://<username>.github.io/<repo-name>/`

## Catatan
- Pastikan file yang dibutuhkan (`index.html`, `style.css`) sudah ada di root repo.
- Jika ingin pakai custom domain, atur juga di menu GitHub Pages.

## Opsi Alternatif
Jika kamu ingin deploy lewat GitHub tetapi tanpa command line, bisa juga:
- Upload file langsung lewat tombol `Add file` > `Upload files`
- Buat file baru dari UI GitHub


Jika kamu mau, saya bisa bantu bikin `.gitignore` dan skrip deploy otomatis juga.