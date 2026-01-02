# 🇹🇷 Turkey BIN List Database 2026 (Türkiye BIN Listesi 2026)

![Data Status](https://img.shields.io/badge/Data-Up%20to%20Date-brightgreen) ![Region](https://img.shields.io/badge/Region-Turkey-red) ![License](https://img.shields.io/badge/License-MIT-blue) ![Size](https://img.shields.io/badge/Records-1400%2B-orange)

**[English]**
A comprehensive, open-source, and up-to-date dataset of **Bank Identification Numbers (BIN)** for Turkey. This repository contains detailed information for over **1,400+** credit and debit card prefixes, including **Issuer Bank**, **Card Network** (Troy, Visa, Mastercard), **Type**, and **Category**.

Perfect for e-commerce validation, fintech applications, payment gateway integrations (Iyzico, PayTR, Stripe, etc.), and data analysis.

**[Türkçe]**
Türkiye'deki banka ve kredi kartlarına ait **BIN (Bank Identification Number)** kodlarının en kapsamlı, açık kaynaklı ve güncel veritabanı. Bu repo, **1.400'den fazla** kart ön eki için **Banka Adı**, **Kart Şeması** (Troy, Visa, Mastercard), **Kart Tipi** ve **Kart Kategorisi** bilgilerini içerir.

Sanal POS entegrasyonları, e-ticaret ödeme sayfaları ve veri analizi projeleri için idealdir.

---

## 📂 Downloads / İndirmeler

You can download the dataset in your preferred format. / Veri setini ihtiyacınız olan formatta indirebilirsiniz.

| Format | File Name | Description / Açıklama | Link |
| :--- | :--- | :--- | :--- |
| **JSON** | `turkey_bin_list.json` | 🚀 Best for Developers & Web Apps | [Download JSON](./turkey_bin_list.json) |
| **Excel** | `turkey_bin_list.xlsx` | 📊 Best for Analysis & Reporting | [Download XLSX](./turkey_bin_list.xlsx) |
| **CSV** | `turkey_bin_list.csv` | 💾 Best for Database Imports (SQL) | [Download CSV](./turkey_bin_list.csv) |

---

## 📊 Data Structure / Veri Yapısı

Each record contains 5 key pieces of information. / Her kayıt 5 temel bilgi içerir.

| Field / Alan | Description (EN) | Açıklama (TR) | Example |
| :--- | :--- | :--- | :--- |
| **BIN** | First 6 digits of the card (IIN) | Kartın ilk 6 hanesi | `554960` |
| **Network** | Card scheme | Kart altyapısı (Visa/Master/Troy) | `MASTERCARD` |
| **Type** | Card type | Kart tipi (Kredi/Banka) | `CREDIT` |
| **Category** | Card tier/segment | Kart segmenti (Gold/Platinum) | `PLATINUM` |
| **Issuer** | The bank name | Banka adı | `TURKIYE GARANTI BANKASI A.S.` |

### Sample JSON Object
```json
[
  {
    "BIN": "405040",
    "Network": "VISA",
    "Type": "DEBIT",
    "Category": "CLASSIC",
    "Issuer": "FUPS BANK ANONIM SIRKETI"
  },
  {
    "BIN": "979288",
    "Network": "TROY",
    "Type": "DEBIT",
    "Category": "STANDARD",
    "Issuer": "TURKIYE VAKIFLAR BANKASI"
  }
]
