# Hi, I'm Yusuf

<details>
<summary>🇹🇷 Türkçe özet için tıklayın</summary>

İstanbul Teknik Üniversitesi, Yapay Zeka ve Veri Mühendisliği bölümünde 4. sınıf öğrencisiyim (tamamı İngilizce eğitim veren bir program). Henüz tek bir alt alana karar vermedim, veri mühendisliği pipeline'ları, klasik makine öğrenmesi, matematiksel optimizasyon ve LLM tabanlı agentic sistemler arasında çalıştım, ve bu projeleri nereye yöneleceğimi anlamak için bir araç olarak kullanıyorum. Aşağıdaki altı proje ilk göstereceğim işler, her birinin arkasında gerçek bir sonuç var, sadece çalışan bir demo değil.

### UYSM: Buğday ve Arpa Verim Analizi

İTÜ Ulusal Yazılım ve Sertifikasyon Merkezi'nde (UYSM), Ar-Ge departmanında yarı zamanlı çalışırken (Aralık 2025 - Haziran 2026) yürüttüğüm bir veri mühendisliği ve analiz projesi; Türkiye'nin ulusal buğday-arpa verim tahmin programından gelen gerçek tarımsal saha ölçüm verisiyle çalışıldı. 291 tutarsız Excel dosyasını doğrulanmış tek bir veri setine dönüştüren uçtan uca bir Python ETL pipeline'ı kuruldu, bu süreçte kaynak tablolardaki 20 gerçek hesaplama hatası bulunup düzeltildi. Çalışma devam ettikçe kapsam büyüdü: ham veri havuzu 79 ile yayılan ~800 ölçüme büyüdü, 90 yinelemeli temizlik sürümünden sonra (her düşen satır gerekçesiyle belgelenerek) 42 ile yayılan, 617 kayıtlık analiz-hazır bir veri setine indirgendi; bitki morfolojisi ile verim arasında istatistiksel olarak anlamlı korelasyonlar bulundu (r'ye kadar 0.72). Kurum onayıyla artık public: [uysm-wheat-barley-yield-analysis](https://github.com/yusuf-oguz/uysm-wheat-barley-yield-analysis)

### Werewolf Agentic Arena

Aynı LLM üzerinde dört standart agentic akıl yürütme desenini (Baseline, Reflection, ReAct, Tree of Thoughts), bir Werewolf (Vampir Köylü/Mafia) sosyal çıkarım oyunu içinde karşılaştırıyor. Oyun ortamının tasarımı var olan çalışmalardan uyarlandı (konuşma sırası Werewolf Arena'dan, oyun durumu tasarımı Xu vd.'den), yeniden icat edilmedi; asıl katkı dört deseni aynı koşullarda çalıştırmak. İstatistiksel olarak anlamlı bir örneklem büyüklüğüne ulaşmanın maliyeti netleşince, 14 oyunda bilinçli olarak durduruldu. [werewolf-agentic-arena](https://github.com/yusuf-oguz/werewolf-agentic-arena), oyun logları [canlı bir dashboard'dan](https://werewolf-agentic-arena.onrender.com/) incelenebilir.

### Data Center Location Optimization

Osmancan Sarı ve Efe Karan Hacımustafaoğlu ile birlikte yürütülen bir takım projesi: Türkiye'nin 81 ili arasından veri merkezi kurulacak en uygun illeri, ikili tamsayılı programlama (PuLP + CBC) ile, beş ağırlıklı yerleşim kriterine (arazi uygunluğu, deprem riski, bağlantı, elektrik maliyeti, soğutma verimliliği) göre seçiyor. İnteraktif, canlı bir uygulama olarak deploy edildi: [data-center-location-optimization](https://github.com/yusuf-oguz/data-center-location-optimization) ([canlı demo](https://data-center-location-optimization.streamlit.app/))

### Micromobility Data Pipeline

Yusuf Öksüzer ile birlikte yürütülen bir takım projesi: İstanbul'da simüle edilmiş bir elektrikli scooter filosu için uçtan uca, konteynerize bir veri mühendisliği pipeline'ı. Bir Python simülatörü PostgreSQL ve Apache NiFi'yi besliyor, NiFi anormallikleri Elasticsearch'e yönlendirip canlı bir Kibana dashboard'u besliyor, Apache Airflow her gece toplu özet çıkarıyor. Tüm sistem tek bir Docker Compose komutuyla ayağa kalkıyor: [micromobility-data-pipeline](https://github.com/yusuf-oguz/micromobility-data-pipeline)

### Anomaly Detection Comparison

Spesifik bir hipotezi test ediyor: backpropagation gerektirmeyen derin öğrenme yöntemleri (PatchCore, PaDiM), standart bir Autoencoder'ın doğruluğunu çok daha az hesaplama maliyetiyle yakalayabilir mi, üstelik klasik yöntemleri (Isolation Forest, One-Class SVM) de geride bırakarak? MVTec AD endüstriyel kusur tespiti benchmark'ında doğrulandı: PatchCore ve PaDiM, Autoencoder'dan çok daha az hesaplamayla %98'in üzerinde AUROC elde etti: [anomaly-detection-comparison](https://github.com/yusuf-oguz/anomaly-detection-comparison)

### Face-Gender-Emotion Categorization

Bir takım projesi: yüzdeki duygusal ifadenin ve cinsiyetin, cinsiyet-kategorileştirme hızını ve doğruluğunu nasıl etkilediğini ölçen, anonimleştirilmiş bir davranışsal deney (PsychoPy ile kuruldu), tekrarlı ölçümler ANOVA'sı (RM-ANOVA) ile analiz edildi. Yüz cinsiyeti ile duygu arasında, kategorileştirme doğruluğu üzerinde güçlü bir etkileşim etkisi bulundu: [face-gender-emotion-categorization](https://github.com/yusuf-oguz/face-gender-emotion-categorization)

**Araçlar:** Günlük olarak Python (pandas, NumPy, scikit-learn, geopandas), optimizasyon için PuLP, interaktif uygulamalar için Streamlit ve Flask (Streamlit Community Cloud ve Render üzerinde deploy edildi), gerektiğinde Docker. Veri mühendisliği altyapısında (Apache NiFi, Airflow, Elasticsearch) ve LLM araçlarında (LiteLLM, OpenAI SDK, AWS Bedrock, DeepSeek API) doğrudan deneyim.

Staj fırsatlarına açığım.

</details>

---

AI & Data Engineering student at Istanbul Technical University (İTÜ), 4th year, 100% English-medium program. I haven't settled on one specific subfield yet, I've worked across data engineering pipelines, classical machine learning, mathematical optimization, and LLM-based agentic systems, and I'm using these projects to figure out where I want to go deeper. Six of them below are the ones I'd point you to first, each with its own real result, not just a working demo.

### UYSM: Wheat & Barley Yield Analysis

A data engineering and analysis project done during a part-time position (Dec 2025 - Jun 2026) at İTÜ's National Software and Certification Center (UYSM), R&D department, working with real agricultural field-measurement data from Turkey's national wheat and barley yield-forecasting program. Built an end-to-end Python ETL pipeline that turned 291 inconsistent Excel files into a validated dataset, catching and fixing 20 real computational errors in the source spreadsheets along the way. The scope grew substantially over time: the raw pool reached about 800 measurements across 79 provinces, and after 90 iterative cleaning versions (every dropped row documented with a reason) it became a 617-record, 42-province analysis-ready dataset, with statistically significant correlations between plant morphology and yield (r up to 0.72). Now public with institutional approval: [uysm-wheat-barley-yield-analysis](https://github.com/yusuf-oguz/uysm-wheat-barley-yield-analysis)

### Werewolf Agentic Arena

Implements and compares four standard agentic reasoning patterns, Baseline, Reflection, ReAct, and Tree of Thoughts, on the same LLM, inside a Werewolf (Mafia) social deduction game. The environment design is adapted from existing research (Werewolf Arena's turn order, Xu et al.'s game-state design), not reinvented; the actual contribution is running all four patterns under matched conditions. Stopped deliberately at 14 games once the cost of reaching a statistically meaningful sample became clear. [werewolf-agentic-arena](https://github.com/yusuf-oguz/werewolf-agentic-arena), game logs browsable in a [live dashboard](https://werewolf-agentic-arena.onrender.com/).

### Data Center Location Optimization

A team project (with Osmancan Sarı and Efe Karan Hacımustafaoğlu) that selects the best provinces among Turkey's 81 for data center placement, using binary integer programming (PuLP + CBC) over five weighted siting criteria: land availability, seismic risk, connectivity, power cost, and cooling efficiency. Deployed as an interactive, live app: [data-center-location-optimization](https://github.com/yusuf-oguz/data-center-location-optimization) ([live demo](https://data-center-location-optimization.streamlit.app/))

### Micromobility Data Pipeline

A team project (with Yusuf Öksüzer): a containerized, end-to-end data engineering pipeline for a simulated electric scooter fleet in Istanbul. A Python simulator feeds PostgreSQL and Apache NiFi, NiFi routes anomalies to Elasticsearch for a live Kibana dashboard, and Apache Airflow runs nightly batch summaries. The whole stack comes up with one Docker Compose command: [micromobility-data-pipeline](https://github.com/yusuf-oguz/micromobility-data-pipeline)

### Anomaly Detection Comparison

Tests a specific hypothesis: can backpropagation-free deep learning methods (PatchCore, PaDiM) match the accuracy of a standard Autoencoder at a fraction of the compute cost, while still beating classical methods (Isolation Forest, One-Class SVM)? Confirmed on the MVTec AD industrial-defect benchmark: PatchCore and PaDiM cleared 98% AUROC with far less compute than the Autoencoder: [anomaly-detection-comparison](https://github.com/yusuf-oguz/anomaly-detection-comparison)

### Face-Gender-Emotion Categorization

A team project: an anonymized behavioral experiment (built with PsychoPy) measuring how a face's emotional expression and gender interact to affect gender-categorization speed and accuracy, analyzed with repeated-measures ANOVA. Found a strong interaction effect between face gender and emotion on categorization accuracy: [face-gender-emotion-categorization](https://github.com/yusuf-oguz/face-gender-emotion-categorization)

Open to internship opportunities.

## Tools

Python day to day (pandas, NumPy, scikit-learn, geopandas), PuLP for optimization, Streamlit and Flask for interactive apps (deployed on Streamlit Community Cloud and Render), Docker when a project calls for it. Some hands-on work with data-engineering infrastructure (Apache NiFi, Airflow, Elasticsearch) and LLM tooling (LiteLLM, OpenAI SDK, AWS Bedrock, DeepSeek API).

## Reach me

https://www.linkedin.com/in/oguz-yusuf/

oguzyu22@itu.edu.tr
