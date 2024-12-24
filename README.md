#                                                WEB SCRAPİNG

## Web Kazıma Nedir?
 Web kazıma, aşağıdakileri toplama sürecini ifade eden bir tekniktir 
web sitelerinden yapılandırılmış veriler. Bu, web sitelerini otomatik olarak tarayarak yapılır. 
Web sayfalarının HTML kodu ve ilgili bilgilerin çıkarılması. Genellikle 
Python gibi programlama dilleri ve kütüphaneler kullanılarak uygulanır 
Beautiful Soup ve Selenium gibi. Web kazıma, büyük ölçekli ve 
manuel veri analizinin zorluklarını ortadan kaldırarak otomatik veri analizi 
toplama. Bu sayede veri toplama gibi çeşitli alanlarda kritik bir rol oynar. 
analitik, makine öğrenimi ve iş zekası.

 Teknik olarak, web kazıma, bir web sayfasını aşağıdaki yöntemlerle elde etmek için tasarlanmış bir süreçtir 
HTTP istekleri göndermek, HTML DOM'u (Belge Nesne Modeli) analiz etmek 
yapısı ve belirli verilerin çıkarılması. Bu süreçte, birçok farklı türde 
metin, resim, video gibi veriler toplanabilir. Toplanan veriler şunları yapabilir 
daha sonra analiz edilmek, görselleştirilmek veya diğer sistemlere entegre edilmek için kullanılabilir



![Web Scraping](https://storage.semalt.com/uploads/articles/52bc1f7c20b1b1a75ca20fffbd210f352.png)



## Hangi Durumlarda Kullanılır?
 Web kazıma, birçok farklı sektörde geniş bir kullanım alanına sahiptir. Bu 
en yaygın kullanım durumları aşağıda listelenmiştir:

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
Web kazıma teknik olarak güçlü bir araçtır, ancak aşağıdaki hususlara dikkat edilmesi gereken bir uygulamadır 
yasal ve etik çerçevede dikkatli bir şekilde ele alınmalıdır.

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
 Beautiful Soup, HTML işlemek için kullanılan Python ile yazılmış bir kütüphanedir 
ve XML dosyaları ve bunlardan belirli bilgileri ayıklayın. Yaygın olarak 
web kazıma projelerinde tercih edilir. Kullanım alanları aşağıdaki gibidir:

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
 Selenium, web tarayıcılarını otomatikleştirmek için güçlü bir araçtır. Güzel'in aksine 
Çorba, sabit HTML içeriği ile sınırlı değildir. Kullanım için idealdir 
Dinamik olarak yüklenen içerik (örneğin, JavaScript ile oluşturulan veriler). 
Selenium, tarayıcıdaki insan davranışını taklit ederek aşağıdaki gibi görevleri yerine getirir 
sayfalarda gezinme, form doldurma ve JavaScript tarafından yüklenen verileri ayıklama.

 ## Güzel Çorba ile Farklılıklar
- **Dinamik İçerik:** Selenium JavaScript tabanlı içeriği işleyebilirken 
Beautiful Soup sadece statik HTML ile çalışır.
- **Performans:** Selenium bir tarayıcıyı simüle ettiği için daha yavaştır. 
Beautiful Soup hızlıdır ancak yalnızca statik içerikle sınırlıdır.
- **Etkileşim:** Selenium, form doldurma, düğme ve diğer etkileşimleri destekler. 
tıklanıyor. Beautiful Soup sadece verileri çeker.

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
- **Statik Sayfalar:** HTML'de yalnızca statik veriler gerekiyorsa, Beautiful Soup bir 
daha iyi bir seçim.
- **Dinamik Sayfalar:** Selenium ile oluşturulan içerikler tercih edilmelidir. 
JavaScript çekilmesi gerekiyor.
- **Etkileşim Gerektiren İşlemler:** Selenium aşağıdaki gibi görevler için kullanılır 
form doldurma ve buton tıklama.

## Örnek Projede Kullanım Senaryosu
 Bir e-ticaret sitesinden ürün bilgilerini çekmek istediğimizi varsayalım:

 **Güzel Çorba:** Fiyatlar ve ürün başlıkları doğrudan sitede mevcutsa kullanılır 
HTML kaynak kodu.
 **Selenium:** Fiyatların ve ürün başlıklarının dinamik olarak yüklenmesi durumunda kullanılır. 
JavaScript.
 **İkisi Birlikte:** Dinamik içerik Selenium ile yüklenir, ardından Güzel 
Çorba sayfayı analiz eder ve verileri çeker
