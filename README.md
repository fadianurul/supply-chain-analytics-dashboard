Supply Chain & Logistics Performance Tracker (15,000+ Orders Analysis)

![Excel](https://img.shields.io/badge/Tools-Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Domain-Supply_Chain_%26_Logistics-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Executive Summary
Proyek ini melakukan analisis komprehensif terhadap **15.000 data pengiriman logistik** untuk mengidentifikasi penyebab utama keterlambatan pengiriman (*delivery delay*), mengukur performa *On-Time Delivery* (OTD Rate), dan menganalisis dampaknya terhadap kepuasan pelanggan (*Customer Satisfaction Score / CSAT*).

Hasil analisis disusun ke dalam sebuah **Interactive Executive Dashboard di Microsoft Excel** yang dilengkapi dengan *Dynamic Slicers*, *Pivot Tables*, *Pivot Charts*, dan *Business Recommendations*.
 Dashboard Preview

`![Logistics Dashboard](dashboard_screenshot.png)`

Key Metrics & Highlights (KPIs)
* **Total Transaksi Pengiriman:** 15,000 Orders
* **Overall On-Time Delivery (OTD) Rate:** **27.9%** *(Kritis / Membutuhkan perbaikan)*
* **Rata-Rata Durasi Keterlambatan:** **16.0 Jam**
* **Rata-Rata Kepuasan Pelanggan (CSAT):** **4.01 / 5.00**

Key Findings (Temuan Utama)

z **Bottleneck Severitas Tinggi pada Layanan Premium:**
   * Layanan pengiriman cepat seperti **Same Day** dan **Express** justru mencatatkan performa OTD terburuk, masing-masing hanya **3.6%** dan **13.9%**.
   * Sebaliknya, layanan **Economy** mencatatkan OTD Rate tertinggi sebesar **51.3%**.

2. **Dampak Keterlambatan Terhadap Kepuasan Pelanggan (CSAT):**
   * Keterlambatan pengiriman berbanding lurus dengan penurunan kepuasan pelanggan. CSAT untuk layanan *Same Day* berada di angka **3.70/5.00**, jauh lebih rendah dibandingkan layanan *Economy* (**4.19/5.00**).

3. **Bottleneck Rute Antar-Wilayah (Regional Route Issues):**
   * Pengiriman dari gudang (*Warehouse Region*) **South** dan **North** menuju wilayah pelanggan (*Customer Region*) **East** dan **Central** merupakan rute dengan OTD Rate terendah (<20%).

Actionable Business Recommendations

1. **Audit & Re-evaluasi SLA Layanan Same Day / Express:**
   * Melakukan audit alur operasional gudang (*Warehouse Processing Time*) untuk mengidentifikasi *bottleneck* sebelum barang diserahkan ke pihak kurir.
2. **Restrukturisasi Alokasi Vendor Logistik pada Rute Kritis:**
   * Mengalihkan kuota pengiriman untuk rute *South $\rightarrow$ East* dan *North $\rightarrow$ Central* ke mitra kurir eksternal dengan *Service Level Agreement* (SLA) yang lebih ketat.
3. **Implementasi Sistem Proaktif Notifications & CSAT Mitigation:**
   * Mengintegrasikan notifikasi otomatis secara *real-time* kepada pelanggan jika estimasi pengiriman mengalami kendala/keterlambatan di atas 2 jam untuk menekan potensi kepuasan pelanggan yang menurun.


🛠️ Data Architecture & Excel Features Used
* **Data Cleaning & Preprocessing:** Formulas (`IF`, `AVERAGE`, `COUNTIF`, String Concatenation `&`).
* **Advanced Pivot Tables & Calculated Fields:** Pembuatan indikator OTD Rate (%) kustom menggunakan *Calculated Field* dan agregasi data bertingkat.
* **Interactive Slicers:** Menghubungkan *Slicers* (*Customer Region*, *Product Category*, *Payment Method*) ke seluruh Pivot Tables menggunakan *Report Connections*.
* **Data Visualization:** Clustered Bar Charts, Column Charts, dan Horizontal Bar Charts untuk pemetaan Top/Bottom Bottleneck Routes.

Repository Structure
```text
├── Supply Chain & Logistics Performance Tracker.xlsx   # File Workbook Utama Excel
├── dashboard_screenshot.png                            # Preview Screenshot Dashboard
└── README.md                                           # Dokumentasi Proyek
