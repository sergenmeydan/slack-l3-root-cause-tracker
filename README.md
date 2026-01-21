# 🤖 Slack L3 Error & Root Cause Tracker

Bu proje, operasyon ekiplerinin Slack üzerinden paylaştığı hata mesajlarını otomatik olarak analiz eden bir **n8n iş akışıdır**. Karmaşık logları saniyeler içinde anlamlı bir rapora dönüştürür.

## 🔥 Temel Özellikler
* **Akıllı Filtreleme:** Sadece kritik kelimeleri (hata, problem, error) içeren mesajlarda devreye girer.
* **Python Mantık Motoru:** Gelen metni tarayarak hatanın Database mi, Network mü yoksa Yetki kaynaklı mı olduğunu anlar.
* **Aksiyon Önerisi:** Analiz sonucunda ekibe "Servisi restart et" veya "DB Pool'u kontrol et" gibi doğrudan çözüm yolları sunar.
* **Döngü Kilidi:** Botun kendi mesajlarını analiz etmesini önleyen özel bir `bot_id` ve başlık kontrolü içerir.

## 🛠️ Nasıl Kurulur?
1. Repodaki `.json` dosyasını indirin.
2. n8n arayüzünden **Import from File** diyerek içeri aktarın.
3. Slack Trigger düğümünde kendi **Credentials** (Kimlik Bilgileri) ayarlarınızı yapın.
4. Akışı **Publish** ederek aktif hale getirin.

⚠️ Not: Güvenlik nedeniyle Slack API anahtarları ve Kanal ID'leri bu JSON dosyasından temizlenmiştir. Akışı içeri aktardıktan sonra kendi Slack bağlantılarınızı kurmanız ve Kanal ID'nizi Slack Trigger ve Send a message düğümlerinde yeniden seçmeniz gerekmektedir.

## 📸 Ekran Görüntüleri
<img width="871" height="322" alt="image" src="https://github.com/user-attachments/assets/26971bc9-7750-4be4-a46b-3fc4c821f60a" />
<img width="538" height="406" alt="image" src="https://github.com/user-attachments/assets/17e55251-8bd7-49cc-8e74-7e86c5722a09" />

