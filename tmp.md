# Assalamualaikum wr wb 
*perkenalkan nama saya yahya saya ingin berbagi tutorial*
___

# Tutorial Branch di Git

Branch (cabang) di Git sangat membantu untuk mengerjakan fitur-fitur baru, memperbaiki bug, atau bereksperimen tanpa mengganggu branch utama (biasanya bernama main/master). Berikut adalah tutorial dasar tentang cara menggunakan branch di Git.

## 1. Melihat Daftar Branch

```bash
git branch
```
Perintah ini akan menampilkan semua branch yang ada di repository lokal Anda. Branch yang sedang aktif akan ditandai dengan tanda *.

## 2. Membuat Branch Baru

```bash
git branch nama-branch-baru
```
Contoh:
```bash
git branch fitur-login
```

## 3. Berpindah ke Branch Lain

```bash
git checkout nama-branch
```
Contoh:
```bash
git checkout fitur-login
```
Atau, mulai Git versi 2.23, bisa juga:
```bash
git switch fitur-login
```

## 4. Membuat dan Langsung Berpindah ke Branch Baru

```bash
git checkout -b nama-branch-baru
```
Contoh:
```bash
git checkout -b fitur-register
```
Atau:
```bash
git switch -c fitur-register
```

## 5. Menggabungkan Branch (Merge)

Setelah selesai mengerjakan pada branch tertentu, Anda dapat menggabungkannya ke branch utama (misal: main):

```bash
git checkout main
git merge nama-branch
```
Contoh:
```bash
git checkout main
git merge fitur-login
```

## 6. Menghapus Branch

Setelah branch tidak diperlukan lagi, Anda bisa menghapusnya:

```bash
git branch -d nama-branch
```
Contoh:
```bash
git branch -d fitur-login
```

## 7. Mengelola Branch di Remote (GitHub)

- **Mendorong branch ke remote:**
  ```bash
  git push origin nama-branch
  ```
- **Menghapus branch di remote:**
  ```bash
  git push origin --delete nama-branch
  ```

## Tips

- Selalu pastikan Anda berada di branch yang benar sebelum melakukan commit.
- Gunakan nama branch yang jelas sesuai dengan fitur atau bug yang sedang dikerjakan.

---

Semoga tutorial ini membantu! 🚀
