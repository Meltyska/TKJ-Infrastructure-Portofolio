# 🧵 Fiber Optic (FO) Physical Troubleshooting & Splicing

## 1. Scope & Technical Overview
Dokumentasi penanganan gangguan fisik pada jaringan serat optik (Fiber Optic). Berfokus pada pelacakan titik *loss*, perbaikan redaman tinggi (*high attenuation*), dan proses terminasi/penyambungan *core* di lapangan.

## 2. Tools & Measuring Equipment
- **Optical Power Meter (OPM):** Mengukur besaran daya ($dBm$) sinyal optik yang diterima.
- **Visual Fault Locator (VFL / Senter Optik):** Mengidentifikasi titik kebocoran laser/serat putus secara visual.
- **Fusion Splicer & Fiber Cleaver:** Pemotongan presisi dan penyambungan *core* menggunakan leburan busur listrik.
- **Fiber Stripper & Isopropyl Alcohol 99%:** Pengupasan lapisan *coating/cladding* dan pembersihan kontaminasi debu pada serat kaca.

## 3. Incident & Troubleshooting Workflow

### Case: Redaman Sinyal Memburuk / Sinyal Drop (LOS)
- **Kondisi / Masalah:** Rx Power pelanggan mendadak drop ke angka $-29\text{ dBm}$ s/d $-32\text{ dBm}$ (standar toleransi ISP: $-15\text{ dBm}$ s/d $-22\text{ dBm}$), menyebabkan koneksi putus-nyambung (*flapping*).
- **Analisa & Diagnosis:**
  1. Pengukuran ulang Rx Power menggunakan OPM pada titik *patch cord* untuk konfirmasi nilai redaman.
  2. Penembakan laser VFL dari titik pigtail ODP/OTB untuk melacak lekukan (*micro-bending*) atau keretakan *core*.
  3. Ditemukan tekukan kabel terlalu tajam (*bending radius* terlanggar) dan ujung konektor SC/UPC kotor terpecam debu.

- **Tindakan Perbaikan:**
  1. Meluruskan alur kabel drop core dan mematuhi batasan *bending radius* (jarak tekukan aman $\ge 30\text{ mm}$).
  2. Memersihkan ujung *ferrule* konektor menggunakan *fiber cleaner cassette* dan alkohol 99%.
  3. Melakukan *re-splicing* pada titik sambungan yang patah menggunakan Fusion Splicer dan dilindungi *protection sleeve*.

- **Hasil Akhir:** Redaman sinyal optik kembali stabil di angka $-18.2\text{ dBm}$. Sinyal optik jernih dan koneksi kembali normal (*UP*).

---

## 4. Field Evidence & Documentation

![TroubleShooting 2](./troubleshoot%20FO%202.jpg)
![TroubleShooting 3](./troubleshoot%20FO%203.jpg)
![TroubleShooting 4](./troubleshoot%20FO%204.jpg)
![TroubleShooting 5](./troubleshoot%20FO%205.jpg)
