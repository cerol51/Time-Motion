# ⏱️ Operasyonel Mükemmellik & Time & Motion İş Gücü Analiz Paneli

Tesis Yönetimi (Facility Management), endüstriyel temizlik ve operasyonel hizmet sektörleri için geliştirilmiş; **Zaman ve Hareket Etüdü (Time & Motion Study)** prensiplerine dayalı, dinamik ve kapsamlı **Norm Kadro (Headcount) ve İş Gücü Planlama Uygulaması**.

🚀 **Canlı Uygulama (GitHub Pages):** [https://cerol51.github.io/Time-Motion/](https://cerol51.github.io/Time-Motion/)

---

## 🌟 Öne Çıkan Yetenekler

* **📊 Canlı Yönetim Panosu (Executive Dashboard):**
  * Tesis Alanı ($m^2$), Aylık Toplam Efor (Saat), Yalın Kadro (FTE), İzin Doldurucu Tampon (Relief Buffer) ve Genel Headcount KPI kartları.
  * Rutin vs. Proje iş yükü dağılımı çubuk grafiği (Bar Chart).
  * 1., 2. ve 3. Vardiya personel dağılımı ve yüzde oranları halka grafiği (Doughnut Chart).
  * **Kat / Bölge (Zon) Analitiği:** Kat ve bölgelerin $m^2$, saat, kadro ve pay kırılımlarını gösteren dinamik tablo ve yatay bar grafik.

* **📚 580+ Gömülü Sektörel Zaman Normu Kütüphanesi:**
  * **5 Temel Sektör:** Hastane, AVM/Mağaza, Okul/Kampüs, Dikey Bina (Plaza/Ofis), Fabrika/Üretim Tesisi.
  * Her sektör için 112 adet standart operasyonel mahal ve makine verim normu.
  * 21 adet ağır bakım ve periyodik proje işi normu (Cila, halı yıkama, dış cephe cam silimi vb.).
  * Norm verilerini satır içi düzenleyebilme, yeni kod ekleme ve fabrika ayarlarına dönebilme.

* **📁 Hazır Sektörel Proje Şablonları (Quick Templates):**
  * 🏥 *Standart 100 Yataklı Hastane Şablonu*
  * 🛍️ *30.000 m² AVM & Yaşam Merkezi Şablonu*
  * 🏢 *10 Katlı Kurumsal Plaza Şablonu*
  * 🏫 *24 Derslikli K12 Kampüs Şablonu*
  * 🏭 *15.000 m² Üretim Tesisi Şablonu*
  * Tek tıkla gerçekçi mahal dağılımları yükleme ve 30 adıma kadar geri alabilme (`Undo/Redo`).

* **📑 Çift Yönlü Excel Entegrasyonu (SheetJS):**
  * **📊 Excel İndir (`exportExcel`):** Tüm saha matrisini ve yönetim özetini içeren iki sayfalı zengin `.xlsx` dosyası oluşturma.
  * **📄 Boş Şablon İndir (`downloadExcelTemplate`):** Sahada veri toplamak için örnek satırlar ve sektör kod rehberi içeren şablon.
  * **⬆ Veri Yükle:** Doldurulan Excel, CSV veya JSON dosyalarını tek tıkla içeri aktarma.

* **🖨️ Kurumsal Yazdırma ve PDF Çıktısı:**
  * Özel `@media print` stilleri ile gereksiz butonları ve filtreleri gizleyen, A4 formatında temiz teklif ve fizibilite raporu çıktısı.

---

## 📐 Matematiksel Hesaplama Modeli

1. **Toplam Efektif Alan:**
   $$\text{Alan}_{\text{toplam}} = \text{Adet} \times \text{Birim Metraj } (m^2)$$

2. **Günlük Frekans:**
   $$F_{\text{günlük}} = \text{Var}_1 + \text{Var}_2 + \text{Var}_3$$

3. **Aylık Toplam Efor (Saat):**
   $$\text{Efor (Saat)} = \frac{\left( \frac{\text{Alan}_{\text{toplam}} \times \text{Zaman Normu (dk)} \times F_{\text{günlük}} \times \text{Aylık Frekans}}{60} \right)}{\text{Performans Oranı} / 100}$$

4. **Yalın Kadro (Base FTE):**
   $$\text{Yalın Kadro} = \frac{\text{Aylık Toplam Efor}}{\text{Personel Aylık Çalışma Günü} \times \text{Günlük Vardiya Saati}}$$

5. **Norm Kadro (Yedek / İzin Payı Dahil):**
   $$\text{Norm Kadro} = \text{Yalın Kadro} \times \left(1 + \frac{\text{Relief Buffer}}{100}\right)$$

6. **Genel Toplam Kadro (Grand Total Headcount):**
   $$\text{Genel Kadro} = \text{Norm Kadro Toplamı} + (\text{Müdür} + \text{Şef} + \text{Makineci} + \text{Camcı})$$

---

## 💻 Teknoloji Yığını

* **HTML5 & Vanilla CSS3** (Flexbox, CSS Grid, CSS Variables)
* **JavaScript (ES6+)**
* **Chart.js** (Veri Görselleştirme)
* **SheetJS / xlsx** (Excel Okuma & Yazma)
* **jQuery & Select2** (Arama Özellikli Seçim Kutuları)
* **Local Storage** (Otomatik Kayıt & İyileştirme Mekanizması)

---

## 🛠️ Yerel Çalıştırma

Uygulama herhangi bir derleme (build) veya sunucu kurulumu gerektirmez.

1. Depoyu klonlayın:
   ```bash
   git clone https://github.com/cerol51/Time-Motion.git
   cd Time-Motion
   ```
2. `index.html` dosyasını doğrudan herhangi bir modern web tarayıcısında açın.
