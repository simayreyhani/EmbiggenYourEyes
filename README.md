# NASA Uzay Görüntü Keşif Platformu 🌌

[![LM Studio](https://img.shields.io/badge/LM%20Studio-Local%20AI-purple)](https://lmstudio.ai/)
[![Ollama](https://img.shields.io/badge/Ollama-Powered-blue)](https://ollama.ai/)
[![Cline](https://img.shields.io/badge/Cline-AI%20Assistant-green)](https://github.com/cline/cline)

NASA Space Apps Challenge 2024 için geliştirilmiş, yerel yapay zeka destekli interaktif uzay görüntü keşif platformu.

## 🎯 Proje Hakkında

Bu proje, NASA Space Apps Challenge kapsamında sunulan **"Leveraging Earth Observation Data for Informed Agricultural Decision-Making"** görevinden ilham alınarak, yerel yapay zeka teknolojileri kullanılarak geliştirilmiştir. Platform, kullanıcıların NASA'nın devasa görüntü veri setlerini keşfetmelerine, yakınlaştırıp uzaklaştırmalarına ve bilinmeyen özellikleri etiketlemelerine olanak tanır.

### NASA Challenge Referansı

NASA'nın uzay misyonları, milyarlarca hatta trilyonlarca piksel içeren yüksek çözünürlüklü görüntüler sunmaktadır:
- Hubble'ın Andromeda galaksisinin 2.5 gigapiksel görüntüsü
- Mars Reconnaissance Orbiter'ın günlük gigapiksel seviyesindeki Mars haritaları
- Lunar Reconnaissance Orbiter'ın Ay yüzeyinin detaylı görüntüleri

Bu platform, bu devasa veri setlerini kullanıcı dostu bir şekilde keşfetmeyi mümkün kılar.

## 🤖 Yerel AI ile Geliştirildi

Bu proje tamamen **yerel yapay zeka** teknolojileri kullanılarak geliştirilmiştir:

### Kullanılan Teknolojiler

- **LM Studio**: Yerel AI model yönetimi ve hosting
  - Model: `openai/gpt-oss-20b` (GGUF formatında)
  - Quantization: IXQFP4
  - Arch: gpt-oss (Tool Use için eğitilmiş)
  - Yerel sunucu: `http://10.31.31.184:1234`

- **Ollama**: AI model çalıştırma altyapısı
  - Entegre model yönetimi
  - Optimize edilmiş inference

- **Cline (VSCode Extension)**: AI destekli kod geliştirme asistanı
  - Otomatik kod üretimi
  - Akıllı tamamlama ve öneriler
  - NASA verilerinin entegrasyonu

### Geliştirme Süreci

1. **Veri Toplama**: NASA'nın açık kaynak veri setleri ve Space Apps Challenge dokümanları incelendi
2. **AI İstemi**: LM Studio üzerinde çalışan yerel AI modeline görev detayları ve gereksinimler verildi
3. **Kod Üretimi**: Cline kullanılarak HTML, CSS ve JavaScript kodu otomatik olarak oluşturuldu
4. **Optimizasyon**: Yerel AI ile iteratif geliştirme ve iyileştirmeler yapıldı

## ✨ Özellikler

### 🔍 İnteraktif Keşif
- Sınırsız zoom (0.5x - 5x arası)
- Sürükle-bırak ile gezinme
- Fare tekerleği ile yakınlaştırma/uzaklaştırma
- Animasyonlu kullanıcı arayüzü

### 🌟 Uzay Cisimleri
Platform şu uzay cisimlerini içerir:
- **Orion Bulutsusu (M42)**: En parlak yıldız oluşum bölgesi
- **Ülker (Pleiades - M45)**: Açık yıldız kümesi
- **Andromeda Galaksisi (M31)**: En yakın sarmal galaksi
- **Yengeç Bulutsusu (M1)**: Süpernova kalıntısı
- **Halka Bulutsusu (M57)**: Gezegen bulutsusu
- **Kartal Bulutsusu (M16)**: "Yaratılış Sütunları"

### 📊 Detaylı Bilgi Paneli
Her uzay cismi için:
- Açıklama
- Uzaklık (ışık yılı)
- Tip
- Keşif tarihi
- Büyüklük

### 🎨 Modern Tasarım
- Gradient renkler ve glow efektleri
- Animasyonlu marker'lar (pulse efekti)
- Glassmorphism stil
- Responsive tasarım

## 🚀 Kurulum ve Kullanım

### Gereksinimler
- Modern web tarayıcı (Chrome, Firefox, Safari, Edge)
- JavaScript desteği

### Yerel Çalıştırma

```bash
# Projeyi klonlayın
git clone https://github.com/kullaniciadi/nasa-space-explorer.git

# Proje dizinine gidin
cd nasa-space-explorer

# index.html dosyasını tarayıcıda açın
# veya bir yerel sunucu başlatın:
python -m http.server 8000
# veya
npx serve
```

### Kullanım

1. **Gezinme**: Fare ile sürükleyerek uzay haritasında dolaşın
2. **Zoom**: 
   - Butonları kullanın (🔍 Yakınlaştır / 🔍 Uzaklaştır)
   - Fare tekerleğini kullanın
3. **Keşif**: Renkli marker'lara tıklayarak cisim detaylarını görün
4. **Sıfırlama**: ↻ Sıfırla butonu ile başlangıç görünümüne dönün

## 📁 Proje Yapısı

```
nasa-space-explorer/
│
├── index.html          # Ana uygulama dosyası
├── README.md           # Proje dokümantasyonu
└── assets/            # (Opsiyonel) Görseller ve kaynaklar
```

## 🛠️ Teknik Detaylar

### Teknolojiler
- **HTML5 Canvas**: Yüksek performanslı görüntüleme
- **Vanilla JavaScript**: Hafif ve hızlı
- **CSS3**: Modern animasyonlar ve efektler
- **Responsive Design**: Tüm ekran boyutlarına uyum

### Performans Optimizasyonları
- Canvas tabanlı rendering
- Efficient marker management
- Lazy loading için hazır altyapı
- Memory-efficient star field generation

## 🎓 NASA Space Apps Challenge

Bu proje, NASA Space Apps Challenge'ın aşağıdaki hedeflerine yanıt vermektedir:

✅ **Kullanıcı Dostu Platform**: Sezgisel arayüz ve kolay navigasyon  
✅ **Zoom Yetenekleri**: Sınırsız zoom ile detay inceleme  
✅ **Etiketleme Sistemi**: İnteraktif marker'lar ve bilgi panelleri  
✅ **Görselleştirme**: Yüksek kaliteli rendering ve efektler  
✅ **Eğitim ve Keşif**: Hem halk hem de araştırmacılar için uygun  

## 🤝 Katkıda Bulunma

Katkılarınızı bekliyoruz! Lütfen şu adımları izleyin:

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/AmazingFeature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Add some AmazingFeature'`)
4. Branch'inizi push edin (`git push origin feature/AmazingFeature`)
5. Pull Request açın

## 📜 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakın.

## 👥 Geliştirici

Bu proje, NASA Space Apps Challenge için yerel AI teknolojileri kullanılarak geliştirilmiştir.

### AI Geliştirme Ortamı
```json
{
  "model": "openai/gpt-oss-20b",
  "format": "GGUF",
  "quantization": "IXQFP4",
  "context_length": 32768,
  "tools": ["LM Studio", "Ollama", "Cline"],
  "local_server": "http://10.31.31.184:1234"
}
```

## 🙏 Teşekkürler

- **NASA** - Açık kaynak veri setleri ve inspirasyon için
- **Space Apps Challenge** - Harika bir etkinlik organizasyonu için
- **LM Studio, Ollama, Cline** - Güçlü yerel AI araçları için
- **Açık Kaynak Topluluğu** - Sürekli destek ve katkılar için

## 📞 İletişim

Sorularınız için:
- GitHub Issues: [https://github.com/simayreyhani/EmbiggenYourEyes]
- Email: [simay.reyhani@stu.bahcesehir.k12.tr]

---

<div align="center">

**🌟 NASA Space Apps Challenge 2024 🌟**

*Made with ❤️ and Local AI*

</div>

## 🔮 Gelecek Planları

- [ ] Gerçek NASA API entegrasyonu
- [ ] Daha fazla uzay cismi ekleme
- [ ] Zaman bazlı görüntü karşılaştırma
- [ ] AI destekli özellik tanıma
- [ ] Çoklu dil desteği
- [ ] Mobil uygulama versiyonu
- [ ] VR/AR desteği
- [ ] Topluluk katkıları için etiketleme sistemi

---

**Not**: Bu proje, NASA Space Apps Challenge için eğitim ve keşif amaçlı geliştirilmiştir. Gerçek bilimsel çalışmalar için NASA'nın resmi platformlarını kullanın.
