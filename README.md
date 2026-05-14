# 🎵 Medya Dosyasından Ses Kırpma Aracı (Audio Splitter)

Bu proje, hem ses hem de video dosyalarından ses izini ayıklayıp, belirlediğiniz sürelerde segmentlere bölen profesyonel, web tabanlı bir araçtır. Tamamen tarayıcı üzerinde çalışır ve dosyalarınız asla bir sunucuya yüklenmez.

[English description below](#english)

---

## 🚀 Öne Çıkan Özellikler

- **Geniş Format Desteği:** 
  - **Ses:** MP3, WAV, M4A, OGG
  - **Video:** MP4, MOV, WEBM (Videolardaki sesi otomatik ayıklar)
- **Akıllı Segmentasyon:** Ses dosyasını belirlediğiniz sürelere (örneğin 20 dakikalık bölümler) böler.
- **Son Segment Birleştirme:** Eğer son parça çok kısaysa (belirlediğiniz minimum sürenin altındaysa), otomatik olarak bir önceki parçaya eklenir.
- **Boyut Optimizasyonu:** Çıktı kalitesini (Düşük, Orta, Yüksek) ayarlayarak dosya boyutunu %80'e varan oranlarda küçültebilirsiniz.
- **Esnek İndirme Seçenekleri:** 
  - Segmentleri tek tek indirme.
  - Tüm segmentleri tek bir **ZIP** dosyasında indirme.
  - **Klasöre Kaydet:** Dosyaları doğrudan bilgisayarınızdaki bir klasöre topluca kaydetme (Chrome/Edge desteği).
- **Gizlilik Odaklı:** Tüm işlemler yerel cihazınızda (client-side) yapılır; internet bağlantısı gerekmez ve verileriniz güvendedir.
- **Görsel Önizleme:** İşlem öncesi segment sayısını ve tahmini dosya boyutunu görebilirsiniz.

## 🛠️ Teknik Detaylar

- **Web Audio API:** Yüksek performanslı ses işleme.
- **JSZip:** Tarayıcı tarafında dinamik ZIP oluşturma.
- **File System Access API:** Klasöre doğrudan yazma desteği.
- **Vanilla JS:** Ekstra bir framework gerektirmeyen saf JavaScript mimarisi.

## 📖 Kullanım Kılavuzu

1. **Dosya Yükleme:** `index.html` dosyasını tarayıcınızda açın ve medya dosyanızı sürükleyip bırakın. (Maks. 500MB)
2. **Ayarları Yapılandırma:**
   - **Segment Süresi:** Her bir ses parçasının kaç dakika olacağını seçin.
   - **Minimum Son Segment:** Son parçanın çok kısa kalmasını istemiyorsanız bu süreyi ayarlayın.
   - **Format & Kalite:** MP3 (optimize) veya WAV seçimi yapın, kalite seviyesini belirleyin.
3. **İşleme:** "Sesi Kırp ve İndir" butonuna tıklayın.
4. **Kaydetme:** İşlem bittiğinde size en uygun indirme yöntemini seçerek dosyalarınızı alın.

---

<a name="english"></a>
# 🎵 Media to Audio Splitter

A professional web-based tool that extracts audio from both audio and video files and splits them into segments based on your preferred duration. It runs entirely in the browser, ensuring your files are never uploaded to a server.

## 🚀 Key Features

- **Wide Format Support:** 
  - **Audio:** MP3, WAV, M4A, OGG
  - **Video:** MP4, MOV, WEBM (Automatically extracts audio from video)
- **Smart Segmentation:** Splits audio into fixed durations (e.g., 20-minute chunks).
- **Last Segment Merging:** If the final piece is too short, it automatically merges with the previous segment.
- **Size Optimization:** Adjust output quality (Low, Medium, High) to reduce file size by up to 80%.
- **Flexible Export Options:** 
  - Download segments individually.
  - Download all segments in a single **ZIP** file.
  - **Save to Folder:** Batch save files directly to a local directory (Supported on Chrome/Edge).
- **Privacy Focused:** All processing is done client-side; no internet connection is required after loading, and your data stays safe.

## 🛠️ Technical Details

- **Web Audio API:** High-performance audio processing.
- **JSZip:** Dynamic ZIP creation on the client side.
- **File System Access API:** Direct folder writing support.

## 📖 How to Use

1. **Upload:** Open `index.html` in your browser and drag & drop your media file. (Max 500MB)
2. **Configure Settings:**
   - **Segment Duration:** Choose the length of each audio piece.
   - **Min Last Segment:** Set a threshold to prevent tiny final segments.
   - **Format & Quality:** Select MP3 (optimized) or WAV and choose the quality level.
3. **Process:** Click the "Trim and Download" button.
4. **Save:** Once finished, choose your preferred download method to save your files.

## 📄 Lisans (License)

Bu proje [MIT](LICENSE) lisansı ile lisanslanmıştır.
