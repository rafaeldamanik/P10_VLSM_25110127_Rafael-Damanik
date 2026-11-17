# Praktikum Jaringan Komputer I — Pertemuan 10
## Implementasi VLSM Menggunakan Cisco Packet Tracer

### Identitas Mahasiswa

| Keterangan | Detail |
|---|---|
| Nama | Rafael Damanik |
| NIM | 25110127 |
| Program Studi | D3 Teknik Komputer |
| Kelas | Semester III — TK Grup D |
| Mata Kuliah | Praktikum Jaringan Komputer I |
| Dosen Pengampu | Juni Ismail, S.Kom., M.Kom. |
| Pertemuan | 10 |

---

## Deskripsi Praktikum

Praktikum ini membahas perancangan dan penerapan **Variable Length Subnet Mask (VLSM)** menggunakan aplikasi Cisco Packet Tracer.

Jaringan dengan alamat dasar `192.168.20.0/24` dibagi menjadi lima segmen berdasarkan kebutuhan host yang berbeda, yaitu Laboratorium, Ruang Dosen, Administrasi, Perpustakaan, dan Link Antar-Router.

## Tujuan

- Memahami konsep dasar subnetting dan VLSM.
- Menentukan prefix dan subnet mask sesuai kebutuhan host.
- Membagi alamat IP menjadi beberapa segmen jaringan.
- Melakukan konfigurasi IP pada perangkat PC.
- Menguji konektivitas antarperangkat menggunakan perintah `ping`.

## Pembagian Alamat VLSM

| Segmen | Kebutuhan Host | Network/Prefix | Subnet Mask |
|---|---:|---|---|
| A — Laboratorium | 50 | `192.168.20.0/26` | `255.255.255.192` |
| B — Ruang Dosen | 26 | `192.168.20.64/27` | `255.255.255.224` |
| C — Administrasi | 12 | `192.168.20.96/28` | `255.255.255.240` |
| D — Perpustakaan | 5 | `192.168.20.112/29` | `255.255.255.248` |
| E — Link Router | 2 | `192.168.20.120/30` | `255.255.255.252` |

## Perangkat dan Software

- Cisco Packet Tracer
- 4 unit Switch 2960
- 10 unit PC-PT
- Kabel Copper Straight-Through
- Kabel Copper Cross-Over

## Pengujian Jaringan

Pengujian dilakukan menggunakan perintah `ping` melalui Command Prompt pada masing-masing PC.

Pengujian meliputi:

1. Konektivitas PC dalam Segmen A.
2. Konektivitas PC dalam Segmen B.
3. Konektivitas PC dalam Segmen C.
4. Konektivitas PC dalam Segmen D.
5. Konektivitas PC dalam Segmen E.
6. Pengujian komunikasi antarsegmen.

**Catatan:** Pada tahap praktikum ini, komunikasi antarsegmen belum tersedia karena konfigurasi router belum dilakukan. Pengaturan gateway disiapkan untuk praktikum pertemuan 12.

## Struktur Repository

```text
P10_VLSM_NIM_RafaelDamanik/
│
├── README.md
├── P10_VLSM_NIM_RafaelDamanik.pkt
├── Laporan_P10_NIM_RafaelDamanik.pdf
│
└── Bukti/
    ├── P10_01_Topologi.png
    ├── P10_02_IP_PC-A1.png
    ├── P10_03_IP_PC-E1.png
    ├── P10_04_Ping_SegmenA.png
    ├── P10_05_Ping_SegmenB.png
    ├── P10_06_Ping_SegmenC.png
    ├── P10_07_Ping_SegmenD.png
    ├── P10_08_Ping_SegmenE.png
    └── P10_09_Antarsegmen.png
```

## Kesimpulan

Melalui praktikum ini, pembagian jaringan menggunakan metode VLSM dapat dilakukan berdasarkan kebutuhan host pada setiap segmen. Setiap segmen memiliki network address, subnet mask, rentang host, dan broadcast address masing-masing.

Konfigurasi dan pengujian dilakukan menggunakan Cisco Packet Tracer sebagai simulasi jaringan komputer.

---

**Politeknik Bisnis Indonesia**  
Program Studi D3 Teknik Komputer  
Tahun 2026