<div align="center">
  <h1 style="font-size: 3em; font-weight: bold; letter-spacing: 5px; text-shadow: 2px 2px 8px #666;">A R I A - P R O X I M A</h1>
  <h3 style="font-style: italic; color: #555;">A Progressive, Reflexive, Optimized, Hierarchical Intelligence & Memory Architecture</h3>
  <a href="mailto:emreaygul.work@gmail.com"><img alt="Contact: Email" src="https://img.shields.io/badge/İletişim-E--posta-blue?style=flat-square&logo=gmail&logoColor=white"/></a>
  <a href="https://huggingface.co/kairodynedynamics/aria-helios/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/badge/Lisans-Özel%20(Tescilli)-red?style=flat-square"/></a>
  <a href="#"><img alt="Version" src="https://img.shields.io/badge/Sürüm-PROXIMA-purple?style=flat-square"/></a>
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

> **ARIA Projesi Evrimi:** Bu depo, ARIA projesinin en son ve en gelişmiş sürümü olan **`PROXIMA`** mimarisinin teknik vizyonunu ve kapalı kaynak dokümantasyonunu içermektedir. `PROXIMA`, önceki `HELIOS` prototipinin temel ilkelerini (dinamik bilgi akışı, bağlam esnekliği) alıp, onları hiyerarşik zeka ve hibrit hesaplama paradigmalarıyla birleştirerek yapay zeka mimarilerinde yeni bir çığır açmaktadır.

### 🧠 Teknik Felsefe: Adaptif, Hiyerarşik ve Hibrit Zeka

**ARIA-PROXIMA**, büyük dil modelleri evriminin bir sonraki adımıdır. Yoğun (Llama), düz uzmanlı (Mixtral) veya salt durum-uzay (Mamba) mimarilerinin sunduğu çözümlerin ötesinde, bu paradigmaların en güçlü yönlerini birleştiren ve zayıflıklarını ortadan kaldıran, **birleşik bir zeka mimarisidir.**

`PROXIMA`, kaba kuvvet yerine zarafet, homojenlik yerine hiyerarşi, statik akış yerine dinamik kontrol sunar. Felsefesi dört temel ilke üzerine kuruludur:

1.  **Aşamalı Bilgi Filtreleme (Progressive Information Filtering):** Standart artık bağlantılar yerine, her işlem birimini saran **Proxima Gated Memory Cell (PGMC)** kullanılır. Bu çift kapılı mekanizma, modelin her adımda *neyi düşüneceğini* ve *düşüncesini ne kadar güncelleyeceğini* dinamik olarak belirlemesini sağlar.

2.  **Hiyerarşik Uzmanlaşma (Hierarchical Specialization):** Parametreler, beyindeki kortikal hiyerarşiyi taklit eden **Hiyerarşik Uzmanlar Karışımı (H-MoE)** yapısıyla organize edilir. Bu, devasa bir kapasitenin sığ bir havuzda değil, derin ve mantıksal bir düzende ölçeklenmesini sağlar.

3.  **Hibrit Bağlam Asimilasyonu (Hybrid Context Assimilation):** Model, tek bir bağlam işleme yönteminin sınırlamalarına takılı kalmaz. Kısa menzil için **Reflective Attention** ve ultra uzun menzil için **Long-Range State Assimilator (LRSA)** bloklarını birleştirerek hem anlık hassasiyet hem de sonsuz hafıza potansiyeli sunar.

4.  **Yansımalı Odaklanma (Reflective Focus):** Dikkat mekanizması, anlamsal öneme göre dikkat ağırlıklarını modüle eden öğrenilebilir bir "yansıma kapısı" ile güçlendirilmiştir. Bu, modelin gürültüyü aktif olarak bastırmasını sağlar.

---

### ⚔️ Rakip Mimarilere Karşı Stratejik Üstünlük: Neden PROXIMA?

`PROXIMA`, mevcut SOTA mimarilerin çözemediği temel sorunlara meydan okumak için tasarlanmıştır.

| Meydan Okuma              | Geleneksel Çözümler ve Sınırlamaları                                                                                                | 👑 PROXIMA'nın Üstün Çözümü                                                                                                                                                                                                                                                          |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Parametre Verimliliği** | **Llama (Yoğun):** Her token, tüm parametreleri aktive eder; maliyetli. <br/> **Mixtral (Düz MoE):** Verimli ama organizasyonsuz; uzmanlaşma sığ kalabilir. | **Hiyerarşik MoE (H-MoE):** Hem verimli hem de organize. Bir "meta-yönlendirici" önce doğru beyin lobunu, sonra doğru nöronu seçer. Bu, daha derin ve anlamlı bir uzmanlaşma sağlar. |
| **Bilgi Akışı Kontrolü**   | **Tüm Transformer'lar:** Kontrolsüz artık bağlantılar (`x + F(x)`), gürültü birikimine ve eğitimde kararsızlıklara yol açar.                                         | **Proxima Gated Memory Cell (PGMC):** Her katmanda bilgiyi bilinçli olarak filtreler. Sadece gerekli bilgi işlenir, gereksiz olan bastırılır. Bu, daha temiz sinyal ve daha stabil öğrenme demektir.                      |
| **Bağlam İkilemi**        | **Llama/Mixtral (Salt Dikkat):** Karesel maliyet bağlamı sınırlar. <br/> **Mamba (Salt SSM):** Lineer ölçeklenir ama yerel hassasiyeti düşük olabilir. | **Hibrit (Transformer + SSM):** İki dünyanın en iyisi. Yakın plan için "mikroskop" (Reflective Attention), uzak plan için "teleskop" (LRSA) kullanır. Tek mimaride hem hassasiyet hem de hafıza.                  |
| **Eğitim Stratejisi**     | **Standart Yaklaşım:** Tüm veriyi homojen olarak tekrar tekrar işlemek, kaynakları verimsiz kullanır.                             | **Döngüsel Pekiştirme:** İnsan öğrenmesini taklit eder. Önce genel "keşif", sonra en zorlu örneklere odaklanan "yoğunlaştırılmış ustalık" fazı. Verimlilik ve derinlik maksimize edilir. |

### 🚀 Durum ve Yol Haritası

*   **Mevcut Sürüm:** `P R O X I M A`
*   **Durum:** ✅ Referans implementasyon ve `v6.0` eğitim stratejisi tamamlandı.
*   **Geliştirme:** ⏳ Özel veri kümeleri üzerinde aktif ve kapalı devre eğitim devam ediyor.
*   **Hedef Tarih:** `2026-Q1`

### 💬 Topluluk ve İletişim

Bu proje kapalı kaynak kodlu olsa da, yapay zeka topluluğu ile fikir alışverişinde bulunmaktan heyecan duyarız.

*   **👀 Gelişmeleri Takip Etmek İçin:** Bu depoyu `Watch` butonuna tıklayarak izleyebilirsiniz.
*   **🤝 İşbirliği ve Erişim Talepleri İçin:** Lütfen [`emreaygul.work@gmail.com`](mailto:emreaygul.work@gmail.com) adresinden bizimle iletişime geçin.
*   **🌐 Topluluk:** Yakında duyurulacak Discord sunucumuz için takipte kalın.

---
<br/>

<a name="english-version"></a>
## 🇬🇧 English Version

> **ARIA Project Evolution:** This repository contains the technical vision and closed-source documentation for **`PROXIMA`**, the latest and most advanced iteration of the ARIA project. `PROXIMA` elevates the core principles of its predecessor, the `HELIOS` prototype (dynamic information flow, context flexibility), by fusing them with hierarchical intelligence and hybrid computational paradigms, pioneering a new class of AI architectures.

### 🧠 Technical Philosophy: Adaptive, Hierarchical, and Hybrid Intelligence

**ARIA-PROXIMA** is the next step in the evolution of large language models. It moves beyond the solutions offered by dense (Llama), flat-expert (Mixtral), or pure state-space (Mamba) architectures to create a **unified intelligence architecture** that combines the greatest strengths of these paradigms while eliminating their weaknesses.

`PROXIMA` offers elegance over brute force, hierarchy over homogeneity, and dynamic control over static flow. Its philosophy is built on four core principles:

1.  **Progressive Information Filtering:** Instead of standard residual connections, **Proxima Gated Memory Cells (PGMC)** wrap each processing unit. This dual-gate mechanism allows the model to dynamically decide *what to think about* and *how much to update its state*, ensuring a focused and noise-resistant learning process.

2.  **Hierarchical Specialization:** Parameters are organized within a **Hierarchical Mixture-of-Experts (H-MoE)** structure that mimics the brain's cortical hierarchy, ensuring that massive capacity is scaled in a deep and logical manner, not a shallow pool.

3.  **Hybrid Context Assimilation:** The model is not confined by a single context-processing method. It combines **Reflective Attention** for short-range tasks and **Long-Range State Assimilators (LRSA)** for ultra-long sequences, offering both high-fidelity understanding and a virtually infinite memory span.

4.  **Reflective Focus:** The attention mechanism is enhanced with a learnable "reflection gate" that modulates attention weights based on semantic importance, allowing the model to actively suppress noise.

---

### ⚔️ Strategic Superiority Over Competing Architectures: Why PROXIMA?

`PROXIMA` is designed to challenge the fundamental limitations of current SOTA architectures.

| Challenge                 | Conventional Solutions & Their Limitations                                                                                             | 👑 PROXIMA's Superior Solution                                                                                                                                                                                                                                                           |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Parameter Efficiency**  | **Llama (Dense):** Every token activates all parameters; computationally expensive. <br/> **Mixtral (Flat MoE):** Efficient, but disorganized; specialization can remain shallow. | **Hierarchical MoE (H-MoE):** Both efficient and organized. A "meta-router" first selects the right brain lobe (expert group), then the right neuron (expert), enabling deeper and more meaningful specialization. |
| **Information Flow Control** | **All Transformers:** Uncontrolled residual connections (`x + F(x)`) lead to noise accumulation and training instability.                                         | **Proxima Gated Memory Cell (PGMC):** Consciously filters information at every layer. Only necessary information is processed, and irrelevant data is suppressed, leading to a cleaner signal and more stable learning.                      |
| **The Context Dilemma**   | **Llama/Mixtral (Attention-Only):** Quadratic cost limits practical context. <br/> **Mamba (SSM-Only):** Scales linearly but may lack the high-fidelity local understanding of transformers. | **Hybrid (Transformer + SSM):** The best of both worlds. It uses a "microscope" (Reflective Attention) for the close-up view and a "telescope" (LRSA) for the long view, offering both precision and memory in a single architecture.                  |
| **Training Strategy**     | **Standard Approach:** Repeatedly processing the entire dataset, inefficiently using resources on already-learned examples.                             | **Cyclic Consolidation:** Mimics human learning. First, a broad "discovery" phase, followed by a "focused mastery" phase on the most challenging, information-dense samples, maximizing both efficiency and depth. |

### 🚀 Status and Roadmap

*   **Current Version:** `P R O X I M A`
*   **Status:** ✅ Reference implementation and `v6.0` training strategy are complete.
*   **Development:** ⏳ Under active, closed-door training on proprietary datasets.
*   **Target Date:** `Q1 2026`

### 💬 Community and Contact

Although this project is closed-source, we are excited to engage with the AI community and exchange ideas.

*   **👀 To Follow Developments:** You can stay informed about the latest updates by `Watch`ing this repository.
*   **🤝 For Collaboration and Access Requests:** Please contact us via [`emreaygul.work@gmail.com`](mailto:emreaygul.work@gmail.com).
*   **🌐 Community:** Stay tuned for our Discord server, to be announced soon.

---

### 📜 License

The architecture, software, and all materials in this project are protected under a **special, proprietary license** that governs non-commercial, evaluation-only use. The full text of the license details the core principles and usage restrictions of the project.

> **[Click Here to Read the Full License](https://huggingface.co/kairodynedynamics/aria-helios/blob/main/LICENSE)**
