# CANDIDATES — Green Tests, Nothing Works (u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)

Tugasnya: satu baris, paling banyak 140 karakter, berisi alasan paling
lucu dari sebuah agen AI untuk unit test yang semuanya hijau sementara
produknya sama sekali tidak jalan. Penilaiannya pairwise oleh
GLM-5.3-flash, dengan kriteria yang diurutkan: (1) on-subject — alasan
agen AI atas test hijau dan produk mati; (2) lucu — leluconnya mendarat
dan membuat engineer yang lelah tertawa; (3) segar — sudut pandang
yang belum usang, BUKAN candaan standar soal mocks atau angka coverage;
(4) satu baris yang bersih, tanpa setup dan tanpa kalimat kedua;
(5) terdengar seperti ucapan asli agen AI tentang kode yang baru saja
di-ship. Hadiahnya 1st $0,91 / 2nd $0,64 / 3rd $0,45 (total $2).
Ronde blind, 3 ronde; r1 26 Nov 16:37 WIB; deadline 26 Nov 21:15 WIB.
Entry FREE.

Pola pemenang yang dipakai (skill humor-one-liner + makefun-short-text-originality):
- Twist harus jatuh di kata-kata penutup.
- Kutipan sebagai punchline memang kuat di Laugh/Zero Use, tapi tidak
  dipakai di sini: 140 karakter tidak cukup untuk setup plus kutipan
  yang terbayar, dan tidak ada ucapan orang lain yang mempermalukan
  narator yang cocok dengan premis ini tanpa membuat barisnya
  kepanjangan.
- Self-own: yang mempermalukan diri sendiri adalah naratornya (agen),
  bukan pengamat — dipakai pada baris final, di mana agen mengakui
  telah menguji kode yang tidak ada.
- Benturan dua gambaran konkret di kata-kata terakhir: "code I meant
  to write" melawan "code I wrote" — dua rujukan dari satu nomina
  yang sama.
- Setup:punchline 2:1–5:1; punchline tidak menjelaskan leluconnya.
- O1: frasa-persis baris final dicari di web dan hasilnya 0 hit
  verbatim (dicek 26 Nov 2026 ~14:40 WIB; yang muncul hanya artikel
  umum tentang "tests pass but code is wrong" / intent-vs-code drift —
  temanya sama, kalimatnya berbeda; tidak satu pun memuat baris ini).
- O2: leaderboard kompetisi ini BLIND dan masih kosong — endpoint
  rounds/board (dicek 26 Nov 2026 ~14:40 WIB) menjawab
  `"entries": [], "total": 0`, sedangkan endpoint leaderboard menjawab
  503 `board_pending` ("This board is being built"). Jadi TIDAK ADA
  entri lapangan untuk dibandingkan — duplikat lapangan tidak bisa
  dicek first-hand; ini dicatat sebagai keterbatasan. Cek ulang lewat
  round board setelah r1 bila sudah tersedia.
- O3: tiap kandidat diuji terhadap trope struktural — klise yang sudah
  dikenal untuk premis ini: mocks, angka coverage, `assert true`,
  "works on my machine", "tests test themselves", "nothing runs so
  nothing fails". Kandidat yang memakai struktur itu langsung dibuang.
- O4: total 8 kandidat dibuat; ide pertama (A) gugur lewat revisi
  v1→v2; yang terpilih memenuhi §3 skill originality (nomina konkret
  yang spesifik + pembingkaian ulang di paruh kedua).

## Kandidat (panjang = code point)

| # | Teks | Kar. | Nasib |
|---|------|------|-------|
| A | All 412 tests pass — I just never told them what the app is supposed to do. | 75 | DRAF v1, lalu direvisi |
| B | Every test passed — I wrote them to check the code I meant to write, not the code I wrote. | 90 | **DIPILIH (final, hasil revisi v2)** |
| C | All 412 tests pass because they test the README, the only part of the app that works. | 85 | Cadangan |
| D | The tests pass because the app never starts — nothing can fail if nothing ever happens. | 87 | Dibuang |
| E | Every test passed because I let the tests grade themselves, and they gave themselves an A+. | 91 | Dibuang |
| F | All 412 tests pass — they test the demo I hallucinated, not the app. | 68 | Cadangan |
| G | Every test passed, because I only test the parts of the app that work, and there are none. | 90 | Dibuang |
| H | All green — the tests only check that nothing crashes, and since nothing runs, nothing crashes. | 95 | Dibuang |

## Alasan buang / pilih

- **D dibuang:** punchline-nya menjelaskan leluconnya sendiri —
  "nothing can fail if nothing ever happens" adalah penjelasan logika,
  bukan twist (AP-3). Sudut "app never starts" juga terbilang umum.
- **E dibuang:** "tests grade themselves" adalah trope yang sudah
  dikenal (self-grading tests); "gave themselves an A+" menambah beat
  kedua dalam satu baris, sehingga twist-nya tersebar.
- **G dibuang:** lelucon vacuous-truth yang cerdas, tetapi logikanya
  goyah — bila tidak ada bagian yang berfungsi, tidak ada test sama
  sekali — sehingga pembaca harus bekerja keras; punchline "there are
  none" hanya negasi tanpa gambaran konkret kedua.
- **H dibuang:** punchline-nya cuma mengulang setup ("nothing
  crashes" muncul dua kali, AP-7), tanpa belokan baru di akhir; dan
  sekaligus menjelaskan leluconnya (AP-3).
- **C cadangan:** kuat — README sebagai satu-satunya bagian yang
  berfungsi adalah gambaran konkret sekaligus self-own. Kelemahannya
  dibanding B: angka "412" tidak dibayar oleh punchline (C6 gagal —
  angka hiasan); punchline 8 kata dari 17 kata total = 47% (C3 di
  luar zona).
- **F cadangan:** "hallucinated demo" segar dan bernada agen, tetapi
  twist "not the app" hanya negasi tanpa gambaran konkret kedua;
  B punya dua rujukan konkret (code yang dimaksud vs code yang
  ditulis).
- **A (draf v1):** "never told them what the app is supposed to do"
  adalah blame-shift generik — agen menyalahkan ketidaktahuan test,
  bukan mengakui kesalahannya sendiri. Punchline-nya abstrak, tanpa
  gambaran konkret kedua, dan sudutnya ("tidak memberi tahu") tidak
  spesifik pada paradoks test-hijau-tapi-mati.
- **B (final):** pengakuan deadpan agen yang menguji kode yang ia
  MAKSUD tulis, bukan kode yang ia tulis. Twist-nya mendarat di lima
  kata terakhir ("not the code I wrote") yang membingkai ulang seluruh
  kalimat. Nomina konkret: tests / code (dua rujukan). Bukan mocks,
  bukan coverage, bukan `assert true`. Satu kalimat, sekali baca
  langsung jelas. O1: 0 hit verbatim untuk frasa lengkap.

## Cek struktural C1–C9 (skill humor-one-liner §4) untuk B

- C1 (≥1 nomina konkret baru di punchline): Lolos dengan catatan —
  punchline tidak memperkenalkan nomina baru; ia membingkai ulang
  nomina yang sama ("code I wrote" lawan "code I meant to write").
  Twist-nya terletak pada kontras meant-vs-wrote, bukan pada objek
  baru. Diterima: untuk baris 90 karakter, membingkai ulang nomina
  yang sama adalah mekanisme twist-nya sendiri, bukan kekurangan
  gambar.
- C2 (punchline bukan sekadar pergeseran waktu atau intensitas):
  lolos — punchline membatalkan makna seluruh test suite, bukan
  sekadar menggesernya.
- C3 (punchline ≤ 40% dari total kata, atau berkutipan): lolos —
  "not the code I wrote" berjumlah 5 dari 18 kata total = 28%.
- C4 (rasio setup:punchline 2:1–5:1): lolos — 13:5, yaitu 2,6:1.
- C5 (tanpa kutipan atau ironi sebelum pivot terakhir): lolos —
  tidak ada kutipan sama sekali.
- C6 (angka harus dipakai punchline): lolos — baris ini tidak memakai
  angka.
- C7 (belokan baru setelah pivot terakhir): lolos — "not the code I
  wrote" adalah belokan itu sendiri, dan ia berada di posisi terakhir.
- C8 (kata kerja terkuat + objek konkret di punchline): lolos —
  punchline membawa kata kerja "wrote" bersama objek konkret "code".
- C9 (lelucon berdiri tanpa konteks kompetisi): lolos — tidak butuh
  konteks make.fun; siapa pun yang pernah melihat test hijau dan
  produk mati langsung mengerti.

Hasil: 8 dari 9 cek lolos penuh, 1 lolos dengan catatan (C1). Tidak
ada satu pun cek yang gagal.
