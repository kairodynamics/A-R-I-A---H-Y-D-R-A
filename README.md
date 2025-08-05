<div align="center">                                          

# A R I A - H E L I O S
### A Hyper-Extensible, Long-context Optimized Self-Regulating Transformer
  
[![Contact: Email]](mailto:emreaygul.work@gmail.com)

</div>

---

<p align="center">
  <strong><a href="#-türkçe-versiyon">🇹🇷 Türkçe Versiyon</a></strong>
     •   
  <strong><a href="#-english-version">🇬🇧 English Version</a></strong>
</p>

---

<a name="türkçe-versiyon"></a>
## 🇹🇷 Türkçe Versiyon

> **Not:** Bu depo, `ARIA-HELIOS` mimarisinin kapalı teknik dökümantasyonunu sunmaktadır. Bu belge, modelin felsefesini, temel bileşenlerini ve tasarım kararlarını detaylandırmak amacıyla oluşturulmuştur.

### 🧠 Teknik Felsefe: Otonom, Verimli ve Esnek Zeka

ARIA-Helios, günümüzün büyük dil modellerinin karşılaştığı verimlilik ve ölçeklenebilirlik zorluklarına yanıt olarak tasarlanmış, son teknoloji bir mimaridir. Geliştirmesi, üç temel ve birbiriyle sinerji içinde çalışan ilkeye dayanmaktadır:

1.  **Kendi Kendini Düzenleyen Bilgi Akışı (Self-Regulating Information Flow):** Standart artık bağlantıları yerine, öğrenilebilir **Kapılı Bellek Birimleri (Gated Memory Units - GMU)** kullanılır. Bu kapılar modelin hangi bilgiyi koruyacağına ve hangisini entegre edeceğine dinamik olarak karar vermesini sağlayarak daha stabil bir eğitim ve daha zengin bir özellik öğrenimi sunar.

2.  **Dinamik Bağlam Esnekliği (Dynamic Context Flexibility):** Modelin anlama kapasitesi, eğitim penceresiyle sınırlı olmamalıdır. **YaRN (Yet another RoPE extensioN method)**'dan ilham alan ölçeklendirme, modelin yeniden eğitime gerek kalmadan, eğitimde gördüğünün çok ötesindeki dizi uzunluklarını etkili bir şekilde işlemesine olanak tanır.

3.  **Maksimum Donanım Verimliliği (Maximum Hardware Efficiency):** Mimarinin her katmanı, modern hızlandırıcılardan (GPU/TPU) maksimum verim almak ve VRAM kullanımını en aza indirmek için tasarlanmıştır. **Gradient Checkpointing, CPU Offloading** ve **FP8 Activation Storage** gibi tekniklerin entegre kullanımı, devasa modellerin daha erişilebilir donanımlarla eğitilmesini mümkün kılar.

### 🛠️ Mimari Planı ve Teknik Bileşenler

ARIA-Helios'un gücü, birbiriyle uyum içinde çalışan modern ve verimli bileşenlerin birleşiminden gelir.

*   #### Gated Memory Units (GMU)
    *   **Ne yapar?** Standart artık bağlantıların yerini alır.
    *   **Nasıl çalışır?** Girdi ve katman dönüşümünü öğrenilebilir bir sigmoid kapısı ile dinamik olarak ağırlıklandırır. Eksi değer ile başlatılan kapılar, modelin önce stabil kimlik bağlantılarını öğrenmesini sağlar.

*   #### Dynamic Context Scaling (YaRN-inspired)
    *   **Ne yapar?** Modelin eğitimde gördüğünden daha uzun metinleri işlemesini sağlar.
    *   **Nasıl çalışır?** RoPE pozisyonel gömmelerinin frekanslarını ve sorgu (query) vektörlerinin genliğini, bağlam genişletme faktörüne göre yeniden ölçekler.

*   #### Grouped-Query Attention (GQA)
    *   **Ne yapar?** Çıkarım hızını artırır ve bellek bant genişliği ihtiyacını azaltır.
    *   **Nasıl çalışır?** Tam sayıda Sorgu (Query) başlığına karşılık daha az sayıda Anahtar (Key) ve Değer (Value) başlığı kullanarak KV-Cache boyutunu dramatik şekilde küçültür.

*   #### Entegre Bellek ve Hesaplama Optimizasyonları
    *   **Ne yapar?** Sınırlı VRAM ile çok büyük modellerin eğitilmesini sağlar.
    *   **Nasıl çalışır?** `Gradient Checkpointing`, `CPU Offload` ve `FP8 Activation Storage` gibi tekniklerin sinerjik kullanımıyla GPU belleğini maksimum verimlilikle yönetir.

### ✨ Temel Farklılıklar ve Geliştirmeler

| Özellik                 | Standart Transformer Yaklaşımı                  | ✅ ARIA-HELIOS Yaklaşımı                                                              |
| ------------------------ | ----------------------------------------------- | ---------------------------------------------------------------------------------- |
| **Bilgi Akışı**          | Statik Artık Bağlantı.          | **Dinamik GMU** ile öğrenilebilir bilgi akış kontrolü.          |
| **Bağlam Penceresi**     | Eğitildiği uzunlukla (örn. 4K token) sınırlıdır. | **Dinamik Ölçekleme (YaRN)** ile çıkarımda bağlamı yeniden eğitime gerek kalmadan genişletebilir. |
| **Dikkat Mekanizması**   | Multi-Head Attention (MHA).                     | **Grouped-Query Attention (GQA)** ile daha hızlı çıkarım ve düşük KV-cache boyutu.   |
| **Donanım Verimliliği**  | Yüksek VRAM tüketimi, pahalı donanım gerektirir. | **Checkpointing, Offload, FP8 Aktivasyonlar** ile entegre ve sinerjik bellek optimizasyonu. |
| **Çıkarım Hızı**         | Standart PyTorch implementasyonları.            | PyTorch 2.0+ **SDPA** (FlashAttention gibi) backend'lerini otomatik kullanarak maksimum hız. |

### 🚀 Durum ve Yol Haritası

*   **Mevcut Sürüm:** `H E L I O S (Hyper-Extensible Long-context Optimized System)`
*   **Durum:** ✅ Mimarinin referans implementasyonu tamamlandı.
*   **Geliştirme:** ⏳ Aktif geliştirme ve kapalı eğitim altında.
*   **Tarih:** `01.08.2025`

### 💬 Topluluk ve İletişim

Bu proje kapalı kaynaklı olsa da, yapay zeka topluluğuyla etkileşim kurmaktan ve fikir alışverişinde bulunmaktan heyecan duyuyoruz.

*   **👀 Gelişmeleri Takip Etmek İçin:** Bu depoyu `Watch` ederek en son güncellemelerden haberdar olabilirsiniz.
*   **🤝 İşbirliği ve Erişim Talepleri İçin:** Lütfen [`emreaygul.work@gmail.com`](mailto:emreaygul.work@gmail.com) üzerinden bizimle iletişime geçin.
*   **🌐 Topluluk:** Yakında duyurulacak Discord sunucumuz için takipte kalın.

---
<br/>

<a name="english-version"></a>
## 🇬🇧 English Version

> **Note:** This repository provides the technical documentation for the `ARIA-HELIOS` architecture, compatible with the provided Python source code. This document was created to detail the model's philosophy, core components, and design decisions.

### 🧠 Technical Philosophy: Autonomous, Efficient, and Flexible Intelligence

ARIA-Helios is a state-of-the-art architecture designed in response to the efficiency and scalability challenges faced by today's large language models. Its development is based on three fundamental and synergistic principles:

1.  **Self-Regulating Information Flow:** Instead of standard residual connections, learnable **Gated Memory Units (GMUs)** are used. These gates allow the model to dynamically decide which information to preserve and which to integrate, leading to more stable training and richer feature learning.

2.  **Dynamic Context Flexibility:** The model's comprehension capacity should not be limited by its training window. Scaling inspired by **YaRN (Yet another RoPE extensioN method)** allows the model to effectively handle sequence lengths far beyond what it has seen during training, without the need for retraining.

3.  **Maximum Hardware Efficiency:** Every layer of the architecture is designed to maximize throughput on modern accelerators (GPU/TPU) and minimize VRAM usage. The integrated use of techniques like **Gradient Checkpointing, CPU Offloading**, and **FP8 Activation Storage** makes it possible to train massive models on more accessible hardware.

### 🛠️ Architecture Blueprint and Technical Components

The power of ARIA-Helios comes from the combination of modern and efficient components working in harmony.

*   #### Gated Memory Units (GMU)
    *   **What it does:** Replaces standard residual connections.
    *   **How it works:** It dynamically weights the input and the layer transformation with a learnable sigmoid gate. The gates are initialized with a negative bias, encouraging the model to first learn stable identity connections.

*   #### Dynamic Context Scaling (YaRN-inspired)
    *   **What it does:** Enables the model to process texts longer than those seen during training.
    *   **How it works:** It rescales the frequencies of RoPE positional embeddings and the magnitude of query vectors according to the context extension factor.

*   #### Grouped-Query Attention (GQA)
    *   **What it does:** Increases inference speed and reduces memory bandwidth requirements.
    *   **How it works:** It dramatically reduces the KV-Cache size by using fewer Key (K) and Value (V) heads than the full number of Query (Q) heads.

*   #### Integrated Memory and Computation Optimizations
    *   **What it does:** Enables the training of very large models with limited VRAM.
    *   **How it works:** It manages GPU memory with maximum efficiency through the synergistic use of techniques like `Gradient Checkpointing`, `CPU Offload`, and `FP8 Activation Storage`.

### ✨ Key Differences and Improvements

| Feature                  | Standard Transformer Approach                   | ✅ ARIA-HELIOS Approach                                                              |
| ------------------------ | ----------------------------------------------- | ---------------------------------------------------------------------------------- |
| **Information Flow**     | Static Residual Connection                      | Learnable information flow control with **Dynamic GMU**.                           |
| **Context Window**       | Limited to training length (e.g., 4K tokens).   | Can extend context at inference time without retraining via **Dynamic Scaling (YaRN)**. |
| **Attention Mechanism**  | Multi-Head Attention (MHA).                     | Faster inference and smaller KV-cache with **Grouped-Query Attention (GQA)**.      |
| **Hardware Efficiency**  | High VRAM consumption, requires expensive hardware. | Integrated and synergistic memory optimization with **Checkpointing, Offload, FP8 Activations**. |
| **Inference Speed**      | Standard PyTorch implementations.               | Maximum speed by automatically using PyTorch 2.0+ **SDPA** backends (like FlashAttention). |

### 🚀 Status and Roadmap

*   **Current Version:** `H E L I O S (Hyper-Extensible Long-context Optimized System)`
*   **Status:** ✅ Reference implementation of the architecture is complete.
*   **Development:** ⏳ Under active development and closed training.
*   **Date:** `01.08.2025`

### 💬 Community and Contact

Although this project is closed-source, we are excited to engage with the AI community and exchange ideas.

*   **👀 To Follow Developments:** You can stay informed about the latest updates by `Watch`ing this repository.
*   **🤝 For Collaboration and Access Requests:** Please contact us via [`emreaygul.work@gmail.com`](mailto:emreaygul.work@gmail.com).
*   **🌐 Community:** Stay tuned for our Discord server, to be announced soon.

---

### 📜 Lisans (License)
> Copyright (c) 2025, ARIA Development Team
> 
> All rights reserved.
> 
> The materials contained in this repository, including but not limited to software, documentation, architectural descriptions, and all other content, are the proprietary property of the ARIA Development Team.
> 
> Without the prior express written permission of the ARIA Development Team, no part of these materials may be copied, reproduced, modified, distributed, reverse-engineered, or transmitted in any form or by any means.
> 
> Access to these materials is provided for informational and evaluation purposes only and does not grant any right of use, license, or ownership.
