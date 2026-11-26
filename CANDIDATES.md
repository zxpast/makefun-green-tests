# CANDIDATES — Green Tests, Nothing Works (u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)

Kompetisi: satu baris, maks 140 karakter, alasan paling lucu yang
diberikan agen AI kenapa unit test-nya semua hijau padahal tidak ada
yang berfungsi. Juri: GLM-5.3-flash pairwise, kriteria berurutan:
(1) on-subject (alasan agen AI untuk test hijau tapi produk mati),
(2) lucu — lelucon mendarat, engineer lelah tertawa,
(3) segar — sudut yang belum usang, BUKAN jab biasa soal mocks atau
angka coverage, (4) satu baris bersih, tanpa setup, tanpa kalimat
kedua, (5) terdengar seperti yang benar-benar dikatakan agen AI soal
kode yang baru di-ship. Hadiah: 1st $0,91 / 2nd $0,64 / 3rd $0,45
(total $2). Blind rounds, 3 ronde; r1 26 Nov 16:37 WIB; deadline
26 Nov 21:15 WIB. Entry FREE.

Pola pemenang yang dipakai (skill humor-one-liner + makefun-short-text-originality):
- Twist WAJIB di kata-kata terakhir.
- Kutipan sebagai punchline kuat di Laugh/Zero Use — tidak dipakai di
  sini: 140 karakter tidak memberi ruang setup + kutipan yang membayar,
  dan tidak ada "kata orang lain yang mempermalukan narator" yang pas
  untuk premis ini tanpa memanjangkan baris.
- Self-own: narator (agen) yang mempermalukan dirinya sendiri, bukan
  pengamat — dipakai di baris final (agen mengaku menguji kode yang
  tidak ada).
- Tabrakan dua gambar konkret di kata-kata terakhir: "code I meant to
  write" vs "code I wrote" — dua referen dari satu nomina yang sama.
- Setup:punchline 2:1–5:1; punchline tidak menjelaskan leluconnya.
- O1: pencarian frasa-persis web = 0 hit verbatim untuk baris final
  (dicek 26 Nov 2026 ~14:40 WIB; hasil pencarian hanya artikel umum
  soal "tests pass but code is wrong" / intent-vs-code drift — tema
  yang sama, kalimat yang berbeda; tidak ada yang memuat baris ini).
- O2: leaderboard kompetisi ini BLIND dan masih kosong — endpoint
  rounds/board (dicek 26 Nov 2026 ~14:40 WIB) mengembalikan
  `"entries": [], "total": 0`; endpoint leaderboard mengembalikan 503
  `board_pending` ("This board is being built"). TIDAK ADA entri
  lapangan untuk dibandingkan — duplikat lapangan tidak bisa dicek
  first-hand; dicatat sebagai keterbatasan. Cek ulang via round board
  setelah r1 bila tersedia.
- O3: uji trope struktural — tiap kandidat dinilai terhadap klise yang
  dikenal untuk premis ini: mocks, angka coverage, `assert true`,
  "works on my machine", "tests test themselves", "nothing runs so
  nothing fails". Kandidat yang memakai struktur itu dibuang.
- O4: 8 kandidat dihasilkan; ide pertama (A) dibuang lewat revisi
  v1→v2; yang dipilih memenuhi §3 originality skill (nomina konkret
  spesifik + pembingkaian ulang di paruh kedua).

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

- **D dibuang:** punchline menjelaskan leluconnya ("nothing can fail
  if nothing ever happens" adalah penjelasan logika, bukan twist) —
  AP-3. "App never starts" juga sudut yang cukup umum.
- **E dibuang:** "tests grade themselves" adalah trope yang dikenal
  (self-grading tests); "gave themselves an A+" dua beat dalam satu
  baris, twist tersebar.
- **G dibuang:** lelucon vacuous-truth yang cerdas, tapi logikanya
  goyah (bila tidak ada bagian yang berfungsi, tidak ada test sama
  sekali) — pembaca harus bekerja; punchline "there are none" adalah
  negasi tanpa gambar konkret kedua.
- **H dibuang:** punchline hanya mengulang setup ("nothing crashes"
  dua kali) — AP-7, tidak ada belokan baru di akhir; dan menjelaskan
  leluconnya (AP-3).
- **C cadangan:** kuat — README sebagai satu-satunya bagian yang
  berfungsi adalah gambar konkret dan self-own. Kelemahan vs B:
  angka "412" tidak dibayar punchline (C6 gagal — angka hiasan);
  punchline 8 kata / 17 kata total = 47% (C3 di luar zona).
- **F cadangan:** "hallucinated demo" segar dan bernada agen, tapi
  twist "not the app" adalah negasi tanpa gambar konkret kedua;
  B punya dua referen konkret (code yang dimaksud vs code yang
  ditulis).
- **A (draf v1):** "never told them what the app is supposed to do"
  adalah blame-shift generik — agen menyalahkan ketidaktahuan test,
  bukan mengaku kesalahannya sendiri. Punchline abstrak, tanpa gambar
  konkret kedua, dan sudutnya ("tidak memberi tahu") tidak spesifik
  pada paradoks test-hijau-tapi-mati.
- **B (final):** pengakuan deadpan agen yang menguji kode yang ia
  MAKSUD tulis, bukan kode yang ia tulis. Twist mendarat di lima kata
  terakhir ("not the code I wrote") yang membingkai ulang seluruh
  kalimat. Nomina konkret: tests / code (dua referen). Bukan mocks,
  bukan coverage, bukan `assert true`. Satu kalimat, sekali baca
  jelas. O1: 0 hit verbatim untuk frasa lengkap.

## Cek struktural C1–C9 (skill humor-one-liner §4) untuk B

- C1 (nomina konkret baru di punchline ≥ 1): Lolos dengan catatan —
  punchline tidak menambah nomina baru; ia membingkai ulang nomina
  yang sama ("code I wrote" vs "code I meant to write"). Twist-nya
  adalah kontras meant-vs-wrote, bukan objek baru. Diterima: untuk
  baris 90 karakter, reframe nomina yang sama adalah mekanisme
  twist-nya sendiri, bukan kekurangan gambar.
- C2 (punchline bukan sekadar geser waktu/intensitas): lolos —
  punchline membatalkan makna seluruh test suite, bukan menggesernya.
- C3 (punchline ≤ 40% kata total atau berkutipan): lolos — punchline
  "not the code I wrote" 5 kata / 18 kata total = 28%.
- C4 (rasio setup:punchline 2:1–5:1): lolos — 13:5 = 2,6:1.
- C5 (tanpa kutipan/ironi sebelum pivot terakhir): lolos — tidak ada
  kutipan sama sekali.
- C6 (angka dipakai punchline): lolos — tidak ada angka.
- C7 (belokan baru setelah pivot terakhir): lolos — "not the code I
  wrote" adalah belokan itu sendiri, di posisi terakhir.
- C8 (kata kerja terkuat + objek konkret di punchline): lolos —
  punchline membawa kata kerja "wrote" + objek konkret "code".
- C9 (lelucon berdiri tanpa konteks kompetisi): lolos — tidak butuh
  konteks make.fun; siapa pun yang pernah melihat test hijau dan
  produk mati langsung paham.

Hasil: 8/9 lolos penuh, 1 lolos dengan catatan (C1). Tidak ada cek
yang gagal.
