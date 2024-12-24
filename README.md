#                                               Web Scraping (Web Kazıma)

## Web Kazıma Nedir?
Web kazıma, web sitelerinden yapılandırılmış verilerin toplanmasını sağlayan bir tekniktir. Bu işlem, web sayfalarını otomatik olarak tarayarak HTML kodu ve ilgili bilgilerin çıkarılmasını içerir. Web kazıma genellikle Python gibi programlama dilleri ve Beautiful Soup ve Selenium gibi kütüphaneler kullanılarak uygulanır. Web kazıma, büyük ölçekli veri toplama süreçlerini hızlandırarak, manuel veri analizinin zorluklarını ortadan kaldırır. Bu nedenle, analitik, makine öğrenimi ve iş zekası gibi çeşitli alanlarda kritik bir rol oynamaktadır.

Teknik açıdan web kazıma, bir web sayfasını elde etmek için HTTP istekleri gönderilmesi, HTML DOM (Belge Nesne Modeli) yapısının analiz edilmesi ve belirli verilerin çıkarılmasını içeren bir süreçtir. Bu süreçle metin, resim ve video gibi çeşitli veri türleri toplanabilir. Elde edilen veriler, analiz, görselleştirme veya diğer sistemlerle entegrasyon için kullanılabilir.



![Web Scraping](https://storage.semalt.com/uploads/articles/52bc1f7c20b1b1a75ca20fffbd210f352.png)



## Hangi Durumlarda Kullanılır?
 Web kazıma, farklı sektörlerde geniş bir kullanım alanına sahiptir. Aşağıda en yaygın kullanım alanları sıralanmıştır:

 **1) E-Ticaret ve Fiyat İzleme:** Şirketler web kazıma yöntemini kullanır 
rakiplerin fiyatlandırma politikalarını izlemek için teknikler. Bu şekilde, dinamik 
fiyatlandırma stratejileri geliştirilebilir ve rekabetçi fiyatlar sunulabilir. 
tüketiciler.

 **2) Haber ve Bilgi Toplama:** Haber ajansları ve içerik 
sağlayıcılar farklı kaynaklardan haber başlıklarını ve içeriklerini derleyebilir.

 **3) Pazar Analizi:** Veri çıkarma, aşağıdakiler hakkında bilgi toplamak için uygulanır 
potansiyel müşteriler, trend analizi yapmak ve pazarı anlamak 
dinamikler.

 **4) Akademik Araştırma ve Veri Analizi:** Araştırmacılar web kazıma yöntemini kullanır 
büyük ölçekli veri kümelerini toplamak ve analiz etmek için teknikler. Özellikle platformlar 
sosyal medya ve haber siteleri gibi büyük veri sağlayan siteler için kullanılır. 
bu amaçla.

 **5) Emlak ve İş İlanları:** Web kazıma aşağıdaki gibi senaryolarda kullanılır 
emlak sitelerinde kiralık veya satılık mülkler hakkında bilgi toplamak 
veya iş ilanlarını analiz etmek.

 **6) Yapay Zeka ve Makine Öğrenimi:** Yapay Zeka ve Makine Öğrenimi için gerekli veri setleri 
model eğitimi kazıma yöntemleriyle elde edilebilir. Örneğin, 
doğal dil işleme (NLP) projeleri için büyük metin veri kümeleri oluşturmak.



## Yasal ve Etik Hususlar
Web kazıma güçlü bir araç olsa da, kullanımında yasal ve etik kurallara dikkat edilmesi gerekmektedir

## 1) Yasal Çerçeve:
- **Kullanım Şartları:** Çoğu web sitesi kazıma işlemine izin verilip verilmediğini açıklar veya 
kullanım koşullarında yer almamaktadır. Bu kurallara uyulmaması şu sonuçlara yol açabilir 
yasal yaptırımlarda.
- **Telif Hakları ve Fikri Mülkiyet:** Aşağıdaki yollarla elde edilen içerik 
kazıma telif hakkı ile korunuyor olabilir. Bunların izinsiz kullanımı 
içerik yasal sorumluluğa neden olabilir.
- **Veri Koruma Kanunları:** Avrupa Birliği'ndeki GDPR gibi düzenlemeler 
ve Amerika Birleşik Devletleri'ndeki CCPA kişisel verileri korumayı amaçlamaktadır. 
bireyler. Bu tür düzenlemelere uyulması zorunludur. 
kazıma işlemleri.

## 2) Etik Konular:
- **Veri Sahibinin Rızası:** Tarafın rızası olmadan kazıma yapılması 
veri sağlamak etik dışı bir davranış olarak kabul edilir.
- **Kaynakların Yüklenmesi:** Bir web sitesinden büyük miktarda verinin çekilmesi 
sık aralıklar sunucu üzerindeki yükü artırabilir ve aşağıdaki sorunlara yol açabilir 
hizmet kesintileri. Bu, kazıma işleminin yapılması gerektiğini vurgular 
sorumlu bir şekilde.
- **Kaynak Gösterme:** Toplanan veriler analiz edilir ve yayınlanırsa, bu bir 
Kaynağın açıkça belirtilmesi etik bir gerekliliktir.


## Beautiful Soup

## Kullanım Amacı
 Beautiful Soup, Python ile yazılmış ve HTML ile XML dosyalarını işlemek için kullanılan bir kütüphanedir. Web kazıma projelerinde yaygın olarak tercih edilen Beautiful Soup'un temel kullanım alanları şunlardır:

- **HTML Ayrıştırma:** Web sitelerinin HTML kodlarını analiz ederek yapılandırılmış veri elde etme 
web sayfaları.
- **Veri Çıkarma:** Belirli HTML etiketlerinden veya özelliklerinden veri çıkarma 
(örneğin div, span, table).
- **Navigasyon:** DOM ağacındaki öğelerde kolay navigasyon ve organizasyon
- **Düzenleme:** HTML veya XML belgelerini düzenleyerek yeni veri yapıları oluşturma

## Temel Özellikler ve Avantajlar
 - **Kullanıcı Dostu API:** Geliştiriciler HTML belgelerinde kolayca gezinebilir ve
 veri ayıklayın.
 - **Esneklik:** Farklı ayrıştırıcılarla çalışabilir (örn. Htm.parser, lxml).
 - **Hız:** Statik web sayfalarında hızlı veri çıkarma.
 - **Hata Toleransı:** Bozuk verilerle çalışırken veri çıkarımını korur
 veya eksik HTML yapıları.
 - **Python Ekosisteminde Uyumluluk:** Python ile kolayca entegre olabilir
 Pandas, NumPy gibi kütüphaneler

 ```python
 from bs4 import BeautifulSoup
import requests

# Web sayfasını indir
url = "https://example.com"
response = requests.get(url)
html_content = response.content

# Beautiful Soup ile HTML içeriğini çözümle
soup = BeautifulSoup(html_content, "html.parser")

# 1. Sayfa başlığını al
page_title = soup.title.string
print(f"Sayfa Başlığı: {page_title}")

# 2. Tüm bağlantıları listele
print("\nSayfadaki Bağlantılar:")
for link in soup.find_all("a"):
    href = link.get("href")
    text = link.text.strip() if link.text else "Bağlantı Metni Yok"
    print(f"- {text}: {href}")

# 3. Tüm görselleri listele
print("\nSayfadaki Görseller:")
for img in soup.find_all("img"):
    img_src = img.get("src")
    img_alt = img.get("alt", "Alt Metin Yok")
    print(f"- {img_alt}: {img_src}")

# 4. Belirli bir HTML öğesini bul (örneğin: bir tablo)
print("\nSayfadaki Tablo Verileri:")
table = soup.find("table")  # İlk tabloyu bulur
if table:
    for row in table.find_all("tr"):
        cells = row.find_all(["th", "td"])
        row_data = [cell.text.strip() for cell in cells]
        print(f"- {row_data}")
else:
    print("Tablo bulunamadı.")

# 5. Özel bir sınıfı olan öğeleri al
print("\nÖzel Sınıf 'featured' Öğeleri:")
featured_items = soup.find_all(class_="featured")
for item in featured_items:
    print(f"- {item.text.strip()}")

# 6. CSS seçicisiyle belirli bir öğeyi seç
print("\nCSS Seçicisi ile Öğe Seçimi:")
css_selected = soup.select_one("div.content > p.intro")
if css_selected:
    print(f"- Seçilen Öğe: {css_selected.text.strip()}")
else:
    print("Seçilen öğe bulunamadı.")
```



## Selenium

## Dinamik Web Sayfalarındaki Rolü
 Selenium, web tarayıcılarını otomatikleştirmek için kullanılan güçlü bir araçtır. 
 Beautiful Soup'tan farklı olarak, dinamik içerikle (JavaScript ile yüklenen veriler gibi) çalışan web sayfalarındaki verileri çıkarmak için idealdir. 
 Selenium, tarayıcıda insan davranışını taklit eder ve sayfalarda gezinme, form doldurma gibi etkileşimleri simüle edebilir..

 ## Beautiful Soup ile Farklılıklar
- **Dinamik İçerik:**  Selenium, JavaScript tabanlı içeriği işleyebilirken, Beautiful Soup yalnızca statik HTML ile çalışır.
- **Performans:** Selenium daha yavaş bir tarayıcı simülasyonu gerektirirken, Beautiful Soup hız konusunda daha etkilidir.
- **Etkileşim:**  Selenium, form doldurma, düğmelere tıklama gibi etkileşimleri desteklerken, Beautiful Soup yalnızca veri çekmeye yöneliktir.

 ```python
 from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
import time

# 1. WebDriver'ı Başlat
driver = webdriver.Chrome()  # Tarayıcıyı başlatır (Chrome kullanılıyor)
driver.maximize_window()

try:
    # 2. Belirli bir URL'ye git
    url = "https://example.com"
    driver.get(url)

    # 3. Sayfa başlığını al ve yazdır
    print(f"Sayfa Başlığı: {driver.title}")

    # 4. Belirli bir öğeyi bul (örneğin: arama kutusu) ve işlem yap
    search_box = driver.find_element(By.NAME, "q")  # Öğe adı 'q' olan arama kutusunu bulur
    search_box.send_keys("Selenium Python")  # Kutucuğa metin girer
    search_box.send_keys(Keys.RETURN)  # Enter tuşuna basar

    # 5. Bir öğenin görünmesini bekle (Explicit Wait)
    wait = WebDriverWait(driver, 10)  # 10 saniye bekler
    results = wait.until(EC.presence_of_element_located((By.ID, "search")))
    print("Arama sonuçları yüklendi.")

    # 6. Arama sonuçlarındaki ilk bağlantıyı tıkla
    first_result = driver.find_element(By.CSS_SELECTOR, "a:first-of-type")
    first_result.click()

    # 7. Yeni sayfada ekran görüntüsü al
    time.sleep(2)  # Sayfanın yüklenmesi için bekle
    driver.save_screenshot("screenshot.png")
    print("Ekran görüntüsü alındı: screenshot.png")

    # 8. Dropdown (Açılır Menü) İşlemleri
    dropdown = driver.find_element(By.ID, "dropdown_id")  # Açılır menüyü bulur
    dropdown.click()  # Menüyü açar
    option = driver.find_element(By.XPATH, "//option[@value='option_value']")  # Belirli bir seçeneği bulur
    option.click()  # Seçeneği seçer

    # 9. JavaScript kodu çalıştır
    driver.execute_script("alert('Selenium ile JavaScript Çalıştı!');")
    time.sleep(2)  # Uyarıyı görmek için bekle
    driver.switch_to.alert.accept()  # Uyarıyı kapatır

    # 10. Çerez Kabul Butonuna Tıklama
    try:
        cookie_button = driver.find_element(By.ID, "cookie-accept")
        cookie_button.click()
        print("Çerez politikası kabul edildi.")
    except:
        print("Çerez kabul butonu bulunamadı.")

finally:
    # 11. Tarayıcıyı kapat
    time.sleep(2)  # İşlemleri görmek için bekle
    driver.quit()
    print("Tarayıcı kapatıldı.")
 ```



 ## Hangi durumlarda hangisi tercih edilmelidir?
- **Statik Sayfalar:** HTML'de yalnızca statik veriler gerekiyorsa, Beautiful Soup daha iyi bir seçimdir.
- **Dinamik Sayfalar:** JavaScript ile yüklenen içerik için Selenium tercih edilmelidir.
- **Etkileşim Gerektiren İşlemler:** Form doldurma, buton tıklama gibi etkileşimler için Selenium kullanılır.

## Örnek Projede Kullanım Senaryosu
 Bir e-ticaret sitesinden ürün bilgilerini çekmek istediğimizi varsayalım:
 
**Beautiful Soup:** Eğer fiyatlar ve ürün başlıkları doğrudan HTML içinde mevcutsa.
**Selenium:** Eğer fiyatlar ve ürün başlıkları JavaScript ile yükleniyorsa.
**İkisini Birlikte Kullanma:** Dinamik içerik Selenium ile yüklenir, ardından Beautiful Soup ile veri çekilir
