<div align="center">

<img src="brosur.jpg" alt="AYBARS AI B.A.R.S. Hybrid Edition" width="420"/>

# 🛡️ AYBARS AI — V12.5 [B.A.R.S. Hybrid Edition]

**A.Y.B.A.R.S.:** *Advanced Yield & Backbone Autonomous Recovery Sentinel*  
*(Gelişmiş Verimlilik ve Omurga Otonom İyileştirme Nöbetçisi)*

[![Edition](https://img.shields.io/badge/Edition-V12.5%20B.A.R.S.%20Hybrid-00FF41?style=for-the-badge&logoColor=black)](https://erdoganvolkan8167-commits.github.io/aybars-ai/)
[![Architecture](https://img.shields.io/badge/Architecture-SNMP--Free%20%7C%20Zero--SQL%20%7C%20Syslog%20514-00BFFF?style=for-the-badge)](https://erdoganvolkan8167-commits.github.io/aybars-ai/)
[![License](https://img.shields.io/badge/License-Commercial%20(AYB--HWID)-FF4444?style=for-the-badge)](mailto:erdoganvolkan8167@gmail.com)
[![Vendors](https://img.shields.io/badge/Multi--Vendor-Aruba%20%7C%20Comware%20%7C%20Cisco%20%7C%20Huawei-4CAF50?style=for-the-badge)](https://erdoganvolkan8167-commits.github.io/aybars-ai/)

[🌐 Canlı Tanıtım Sitesi](https://erdoganvolkan8167-commits.github.io/aybars-ai/) • [🇹🇷 Türkçe Tanıtım](#-türkçe-genel-bakış) • [🇬🇧 English Overview](#-english-overview) • [📩 Kurumsal Demo](#-kurumsal-demo-ve-lisanslama--enterprise-demo)

</div>

---

## 🇹🇷 Türkçe Genel Bakış

**AYBARS AI V12.5 [B.A.R.S. Hybrid Edition]**; hastaneler, kamu kurumları ve büyük ölçekli kampüs ağları için geliştirilmiş, ağır SQL veritabanları veya karmaşık SNMP/MIB yapılandırması gerektirmeyen **yapay zeka destekli otonom ağ izleme, 1-2 saniyede gerçek zamanlı Syslog alarmı, kendi kendini iyileştirme (Self-Healing) ve aktif müdahale** platformudur.

Piyasadaki klasik NMS yazılımları yalnızca pasif grafikler çizerken, **AYBARS AI** doğrudan kıdemli bir ağ mühendisi gibi çoklu marka CLI (SSH/Telnet) üzerinden switch'lerle konuşur; arızayı nokta atışı tespit eder ve tek tuşla müdahale imkanı sunar.

### 🚀 Öne Çıkan Çekirdek Yetenekler

* **📡 1-2 Saniyede Anlık Syslog (UDP 514) Kriz Bildirimi:** Periyodik tarama sırasını beklemeden switch'lerden gelen `BPDU-Protection`, `Bpdu-Error`, `Loop-Protect` ve `MAC_FLAPPING` paketlerini gerçek zamanlı yakalar; 5 dakikalık spam kalkanıyla anında HTML acil e-posta gönderir.
* **🌪️ 5 Katmanlı B.A.R.S. Loop Avcısı:** Aruba AOS-CX (`Bpdu-Error`, `Loop-Protect`, `Self-LLDP`) ve HP/H3C Comware 7 (`BPDU-Protection`, `STP Down-Port`, `Loopback-Detection`, `Self-LLDP`) katmanlarını eşzamanlı tarayarak köprülenen port çiftlerini (`Port X <---> Port Y`) nokta atışı yakalar.
* **🛡️ 2 Aşamalı Retry & Sıfır Gürültü Politikası:** Anlık SSH zaman aşımında yanlış "DOWN" alarmı üretmemek için 5 saniye beklemeli doğrulama yapar. Access Point kaynaklı `Giants (MTU 1500)` ve hız farkı kaynaklı `Dropped 0 (TX Buffer)` kayıtlarını eler; yalnızca eşik üstü (**+100**) gerçek fiziksel kablo/SFP arızalarında alarm verir.
* **♻️ 15 Dakika Otonom İyileşme (Self-Healing):** Döngü oluşturan kablo fiziksel olarak çıkarıldığında, kilitlenen kenar portlar yönetici müdahalesine gerek kalmadan 900. saniyede kendiliğinden devreye girer.
* **🌡️ Proaktif Sensörler (SFP DOM & DHCP'siz ARP Bekçisi):** Fiber modüllerin sıcaklık (°C) ve Rx/Tx desibel (dBm) zayıflamalarını CRC patlamadan önce raporlar; merkez DHCP erişimi olmadan statik IP/MAC çakışmalarını ve korsan kenar portu tespit eder.
* **⚡ Tek Tuşla Aktif Müdahale:** Web arayüzünden **PoE Kamera/AP Şoklama (Kapat/Aç)**, **Port Karantina (Shutdown)**, **VLAN Atama**, **Evrensel IP/MAC Bulucu**, **Toplu Konfigürasyon (Mass-Config)** ve **Tek Tıkla Tüm Ağ Yedekleme (.ZIP)**.
* **🧠 Yapay Zeka Kriz Masası & Türkçe Sesli Anons:** Deterministik Delta çıktıları üzerinden kök neden analizi yapar, kritik bulguları kırmızı alarm kutularıyla vurgular ve Türkçe sesli özetler.

### ⚔️ Geleneksel NMS Yazılımları ile Farkı

| Özellik / Yetenek | Klasik NMS (SolarWinds / PRTG / OpManager / Zabbix) | AYBARS AI V12.5 [B.A.R.S. Hybrid] |
| :--- | :--- | :--- |
| **Kurulum & Altyapı** | SQL Veritabanı, SNMP v2/v3 ve MIB kütüphaneleri şarttır. | **SNMP-Free & Zero-SQL:** Doğrudan SSH/Telnet ile 5 dakikada hazır. |
| **Loop Tepki Süresi** | Port kapandığında "Port Down" sanarak sessiz kalır. | **1-2 Saniye (Anlık UDP 514 Syslog) + 5 Katmanlı Avcı.** |
| **Yanlış Alarm Koruması** | Anlık gecikmelerde ve paket düşmelerinde spam mail atar. | **2 Aşamalı Retry + Zero-Noise Delta (+100):** `Dropped 0` ve `Giants` elenir. |
| **Aktif Müdahale** | Sadece izler; müdahale için PuTTY / CLI gerekir. | **Tek Ekranda Müdahale:** PoE Şoklama, Port Karantina, Mass-Config ve Toplu Yedek. |
| **Güvenlik & Lisans** | Ağır sunucu ve modül başına yüksek lisans maliyeti. | `AYB-HWID` donanım kilidi, Anti-Rollback, Brute-Force koruması, `shell=False` zırhı. |

### 🖧 Desteklenen Switch Markaları (Multi-Vendor CLI)

* **Aruba AOS-CX (SSH):** 6100, 6200F, 6300, 8100, 8325 Serisi
* **HP / H3C Comware v5 & v7 (SSH / Telnet):** 5120, 5130, 5140 EI/SI, 5500 Serisi
* **Cisco IOS / IOS-XE (SSH):** Catalyst 2960, 3650, 3850, 9200, 9300 Serisi
* **Huawei VRP (SSH):** CloudEngine S5700, S5720, S6720 Serisi
* **HP ProCurve / ArubaOS-Switch (SSH):** 2530, 2540, 2920, 2930F Serisi

---

## 🇬🇧 English Overview

**AYBARS AI V12.5 [B.A.R.S. Hybrid Edition]** (*Advanced Yield & Backbone Autonomous Recovery Sentinel*) is an enterprise-grade, **SNMP-free and Zero-SQL** autonomous network protection, real-time Syslog alerting, self-healing, and crisis management platform built for hospitals, government institutions, and multi-vendor campus networks.

### Key Highlights
* **Real-Time UDP 514 Syslog Listener (1-2s Response):** Captures `BPDU-Protection`, `Bpdu-Error`, `Loop-Protect`, and `MAC_FLAPPING` traps in real time with built-in 5-minute anti-spam cooldown and CLI noise filtering.
* **5-Layer B.A.R.S. Loop Hunter:** Detects error-disabled ports, Comware `STP Down-Port`, `Loopback-Detection`, and `Self-LLDP` physical cable bridges across heterogeneous edge switches.
* **2-Stage Retry & Deterministic Zero-Noise Delta:** Prevents false DOWN alerts via 5-second retry verification and filters out TX buffer drops (`Dropped 0`) and AP `Giants (MTU 1500)`, alerting strictly on verified physical CRC/Input errors.
* **Proactive Hardware Telemetry:** Optical SFP DOM/DDM laser attenuation tracking and DHCP-less Core ARP conflict detection.
* **One-Click Remediation:** Remote PoE power cycling, instant port quarantine, universal IP/MAC edge-port pinpointing, Mass-Config push, and automated multi-switch `.ZIP` backup.

---

## 📩 Kurumsal Demo ve Lisanslama / Enterprise Demo

> ⚠️ **Ticari Lisans Bildirimi:** Bu depo yalnızca **AYBARS AI** mimari tanıtım ve dokümantasyon vitrinidir. Yazılım; sunucu donanım kimliğine (`AYB-HWID`) bağlı süreli `AYBARS-PRO` ticari lisansı ile şifreli paket olarak teslim edilir.

* **Geliştirici / Architect:** Volkan Erdoğan — *Enterprise Network Security & AI Automation*
* **Web Tanıtım Sayfası:** [https://erdoganvolkan8167-commits.github.io/aybars-ai/](https://erdoganvolkan8167-commits.github.io/aybars-ai/)
* **E-Posta / Demo Talebi:** [erdoganvolkan8167@gmail.com](mailto:erdoganvolkan8167@gmail.com)
* **LinkedIn:** [linkedin.com/in/volkan-erdoğan-9665641b5](https://www.linkedin.com/in/volkan-erdo%C4%9Fan-9665641b5)

---

<div align="center">
  <sub>© 2026 Volkan Erdoğan | AYBARS AI V12.5 [B.A.R.S. Hybrid Edition]. Tüm Hakları Saklıdır / All Rights Reserved.</sub>
</div>
