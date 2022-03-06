# Latihan Vite Vue TypeScript - Range Angka

Ini aplikasi untuk tambah kurang angka sederhana antara 0 - 10. Kalau < 0 tombol kurang ke disabled, kalau > 10 tombol tambah ke disabled.

Fungsi yang dipakai ada `ref` (untuk angka reactivenya) sama `watch` (untuk cek disablednya). `onMounted` cuma pemanis aja :smile:

Ceknya [disini](https://ken-diva.github.io/vite-range-angka/) (masi error)

Kalau baru clone, jalanin
- npm i
- npm run dev (running local)

note* 
- ini belum pake css sama sekali. kedepannya mungkin ditambahin (ga janji tapi)
- ketik ini untuk buat sub branch untuk keperluan deploy
  - `git subtree push --prefix dist origin 'nama_branch'`
- youtube deploy tutorial [dimari](https://www.youtube.com/watch?v=yo2bMGnIKE8)

-- 6 Maret 2022