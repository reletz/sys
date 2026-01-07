# Panduan Penggunaan Snippet Cheatsheet

### 1. Instalasi Snippet

1. Simpan file `cheatsheet.css` ke dalam folder `.obsidian/snippets/` di dalam vault Anda.
    
2. Buka Obsidian, masuk ke `Settings` > `Appearance`.
    
3. Scroll ke bawah ke bagian `CSS Snippets`, lalu aktifkan `cheatsheet`.
    

### 2. Cara Penggunaan di Catatan

Untuk mengaktifkan layout cheatsheet, tambahkan `cssclasses: cheatsheet` pada bagian _frontmatter_ catatan Anda.

Untuk memberi warna pada kartu, **tambahkan tag khusus** di akhir baris pertama dari setiap item list utama. Tag ini tidak akan terlihat di kartu.

### Contoh Struktur Markdown (Yang Benar):

Gunakan tag seperti `#card-blue`, `#card-green`, dll.

```
---
cssClasses: cheatsheet
---

# Linux Command Cheatsheet

## Basic Commands

- **ls - list directory contents** #card-blue
    - `ls -l` untuk format panjang
    - `ls -a` untuk menampilkan file tersembunyi
- **cd - change directory** #card-green
    - `cd ~` untuk ke home directory
    - `cd ..` untuk naik satu level
- **mkdir - make directory** #card-red
    - `mkdir folder_baru`
- **touch - create a file** #card-yellow
    - `touch file_baru.txt`

## File Operations

- **cp - copy files** #card-purple
    - `cp source.txt destination.txt`
- **mv - move or rename files** #card-orange
    - `mv old_name.txt new_name.txt`
```