# 🇮🇷 Iranian Holiday Dataset (Solar Year 1404 / Gregorian 2025)

This repository contains a clean, structured dataset of Iranian holidays and cultural/religious events for the year 1404 (2025 Gregorian), extracted and standardized from [time.ir](https://time.ir). It includes exact dates in the **Shamsi (Solar Hijri)**, **Ghamari (Lunar Hijri)**, and **Gregorian** calendars, along with metadata indicating whether a day is officially a public holiday and what kind of event it represents.

---

## 📦 Dataset Overview

| Column Name    | Description |
|----------------|-------------|
| `shamsi`       | Date in Persian (Solar Hijri) calendar |
| `ghamari`      | Date in Islamic (Lunar Hijri) calendar |
| `miladi`       | Date in Gregorian calendar |
| `Event Title`  | Description of the event or holiday in Persian |
| `Holiday`      | `1` if it is an official public holiday, otherwise `0` |
| `flag`         | Categorization of the event type (see below) |

---

## 🏷️ Flag Meaning

| Flag | Meaning                       |
|------|-------------------------------|
| 0    | National or cultural event    |
| 1    | Religious/Islamic occasion    |
| 2    | International/global day      |

---

## 📊 Example Data

```plaintext
shamsi      | ghamari     | miladi     | Event Title                       | Holiday | flag
------------|-------------|------------|-----------------------------------|---------|------
1404/01/01  | 1446/9/21   | 2025/03/21 | جشن نوروز/جشن سال نو              |    1    |   0
1404/01/01  | 1446/9/21   | 2025/03/21 | روز جهانی نوروز                   |    0    |   2
1404/01/02  | 1446/9/22   | 2025/03/22 | شهادت حضرت علی (ع)                |    1    |   1
