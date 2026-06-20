# 🧠 AI Sentiment Analysis (Duygu Analizi)

Bu uygulama, girilen Türkçe veya İngilizce metinlerin duygu durumunu (**Pozitif / Negatif / Nötr**) yapay zeka kullanarak analiz eder. Projede ana motor olarak **Google Gemini AI (gemini-2.5-flash)** kullanılmaktadır; API anahtarı sağlanmadığı durumlarda ise kural tabanlı (heuristic) kelime analizi devreye girmektedir.

---

## 🚀 Özellikler
- **Gemini AI Entegrasyonu:** Metnin bağlamını anlayarak gelişmiş duygu analizi yapar.
- **Yedek Analiz Mekanizması:** API anahtarı olmadığında veya limit aşımında kelime eşleştirme (Heuristic) yöntemiyle kesintisiz çalışır.
- **Streamlit Arayüzü:** Hızlı, modern ve kullanıcı dostu web arayüzü.
- **Canlı Yayın Hazır:** Streamlit Cloud üzerinde doğrudan çalıştırılmaya uygun yapı (secrets desteği).

---

## 🛠️ Kurulum ve Yerel Çalıştırma

### 1. Projeyi Klonlayın
```bash
git clone https://github.com/aysebolat1721-blip/nlp-sentiment-projesi-02-127.git
cd nlp-sentiment-projesi-02-127
```

### 2. Bağımlılıkları Yükleyin
```bash
pip install -r requirements.txt
```

### 3. API Anahtarını Tanımlayın
Proje dizininde `.env` adında bir dosya oluşturun ve Google Gemini API anahtarınızı ekleyin:
```env
API_KEY=your_gemini_api_key_here
```

### 4. Uygulamayı Başlatın
```bash
streamlit run streamlit_app.py
```

---

## ☁️ Streamlit Cloud Canlıya Alma (Deployment)

Uygulamayı Streamlit Cloud üzerinde canlıya alırken şu adımları izleyin:
1. [Streamlit Share](https://share.streamlit.io/) sitesine gidin ve GitHub hesabınızla giriş yapın.
2. **"New app"** butonuna tıklayın.
3. Repository olarak `aysebolat1721-blip/nlp-sentiment-projesi-02-127` seçin.
4. Main file path kısmına `streamlit_app.py` yazın.
5. **Advanced Settings** butonuna tıklayıp **Secrets** kısmına Gemini API anahtarınızı şu şekilde ekleyin:
   ```toml
   API_KEY = "your_actual_gemini_api_key_here"
   ```
6. **"Deploy!"** butonuna tıklayarak uygulamanızı canlıya alın.

---
Geliştiren: Nejdet TUT | Geliştirme Tarihi: Haziran 2026
