# Daftar Kode Akun Kas Kecil

Daftar ini menjadi rujukan saat mencatat transaksi pada berkas `jurnal-umum.csv`. Setiap pengeluaran dicatat pada kode akun beban yang sesuai, dengan pasangan kredit pada akun kas kecil.

| Kode | Nama Akun |
|---|---|
| 1101 | Kas Kecil |
| 5201 | Beban Alat Tulis Kantor |
| 5202 | Beban Materai dan Perangko |
| 5203 | Beban Konsumsi Rapat |
| 5204 | Beban Pengiriman Dokumen |
| 5205 | Beban Fotokopi dan Penggandaan |
| 5210 | Beban Transportasi dan Parkir |

## Cara mencatat

Setiap transaksi ditulis dalam dua baris. Baris pertama mencatat beban pada sisi debit, baris kedua mencatat pengurangan kas kecil pada sisi kredit dengan nominal yang sama.

Contoh pembelian tinta printer senilai Rp 70.000:

```
2026-09-22,5201,Pembelian tinta printer,70000,0
2026-09-22,1101,Pembayaran tinta printer,0,70000
```

Kolom yang tidak terisi diberi angka nol, bukan dikosongkan, agar jumlah kolom setiap baris tetap sama.
