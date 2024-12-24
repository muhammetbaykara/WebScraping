#                                                WEB SCRAPİNG

## What is Web Scraping?
 Web scraping is a technique that refers to the process of collecting 
structured data from websites. This is done by automatically scanning the 
HTML code of web pages and extracting relevant information. It is usually 
implemented using programming languages such as Python and libraries 
such as Beautiful Soup and Selenium. Web scraping enables large-scale and 
automated data analysis by eliminating the challenges of manual data 
collection. In this way, it plays a critical role in various fields such as data 
analytics, machine learning and business intelligence.

 Technically, web scraping is a process designed to source a web page by 
sending HTTP requests, analyze the HTML DOM (Document Object Model) 
structure and extract specific data. In this process, many different types of 
data can be collected, such as text, images, video. The collected data can 
then be used to be analyzed, visualized or integrated into other systems

![Web Scraping](https://storage.semalt.com/uploads/articles/52bc1f7c20b1b1a75ca20fffbd210f352.png)



## In Which Situations Is It Used?
 Web scraping has a wide range of uses in many different industries. The 
most common use cases are listed below:

 **1) E-Commerce and Price Monitoring:** Companies use web scraping 
techniques to track competitors' pricing policies. In this way, dynamic 
pricing strategies can be developed and competitive prices can be offered to 
consumers.

 **2) News and Information Aggregation:** News agencies and content 
providers can compile news headlines and content from different sources.

 **3) Market Analysis:** Data extraction is applied to gather information about 
potential customers, perform trend analysis and understand market 
dynamics.

 **4) Academic Research and Data Analysis:** Researchers use web scraping 
techniques to collect and analyze large-scale datasets. Especially platforms 
that provide large data, such as social media and news sites, are used for 
this purpose.

 **5) Real Estate and Job Postings:** Web scraping is used in scenarios such as 
collecting information about properties for rent or sale on real estate sites 
or analyzing job postings.

 **6) Artificial Intelligence and Machine Learning:** The datasets needed for 
model training can be obtained through scraping methods. For example, 
creating large text datasets for natural language processing (NLP) projects.



## Legal and Ethical Considerations
Web scraping is a technically powerful tool, but it is a practice that needs to 
be handled carefully within a legal and ethical framework.

## 1) Legal Framework:
- **Terms of Use:** Most websites disclose whether scraping is permitted or 
not in their terms of use. Failure to comply with these rules may result 
in legal sanctions.
- **Copyrights and Intellectual Property:** Content obtained through 
scraping may be protected by copyright. Unauthorized use of such 
content may result in legal liability.
- **Data Protection Laws:** Regulations such as GDPR in the European Union 
and CCPA in the United States aim to protect the personal data of 
individuals. It is mandatory to comply with such regulations during 
scraping operations.

## 2) Ethical Issues:
- **Consent of the Data Subject:** Scraping without the consent of the party 
providing the data is considered unethical behavior.
- **Loading of Resources:** Pulling large amounts of data from a website at 
frequent intervals can increase the load on the server and lead to 
service interruptions. This emphasizes that scraping should be done 
responsibly.
- **Citing the Source:** If the collected data is analyzed and published, it is an 
ethical requirement to clearly identify the source.



## Beautiful Soup

## Intended Use
 Beautiful Soup is a library written in Python that is used to process HTML 
and XML files and extract certain information from them. It is widely 
preferred in web scraping projects. Its usage areas are as follows:

- **HTML Parsing:** Obtaining structured data by analyzing the HTML code of 
web pages.
- **Data Extraction:** Extracting data from specific HTML tags or properties 
(e.g. div, span, table).
- **Navigation:** Easy navigation and organization of elements in the DOM tree
- **Editing:** Create new data structures by editing HTML or XML documents

##  Key Features and Benefits
 - **User FriendlyAPI:** Developers can easily navigate HTML documents and
 extract data.
 - **Flexibility:** Can work with different parsers (e.g. Htm.parser, lxml).
 - **Speed:** Fast data extraction on static web pages.
 - **FaultTolerance:** Maintains data extraction when working with corrupted
 or missing HTML structures.
 - **Compatibility in Python Ecosystem:** It can easily integrate with Python
 libraries such as Pandas, NumPy

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

##  Role in Dynamic Web Pages
 Selenium is a powerful tool for automating web browsers. Unlike Beautiful 
Soup, it is not limited to fixed HTML content. It is ideal for handling 
dynamically loaded content (for example, data generated with JavaScript). 
Selenium mimics human behavior in the browser, performing tasks such as 
navigating pages, filling out forms, and extracting data loaded by JavaScript.

 ##  Differences with Beautiful Soup
- **Dynamic Content:** Selenium can handle JavaScript-based content, while 
Beautiful Soup only works with static HTML.
- **Performance:** Selenium is slower because it simulates a browser. 
Beautiful Soup is fast but limited to static content only.
- **Interactivity:** Selenium supports interactions such as form filling, button 
clicking. Beautiful Soup only pulls data.

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



 ## Which one should be preferred in which situations?
- **Static Pages:** If only static data in HTML is required, Beautiful Soup is a 
better choice.
- **Dynamic Pages:** Selenium should be preferred if content created with 
JavaScript needs to be pulled.
- **Transactions Requiring Interaction:** Selenium is used for tasks such as 
form filling and button clicking.

## Usage Scenario in a Sample Project
 Suppose we want to pull product information from an e-commerce site:

 **Beautiful Soup:** Used if prices and product titles are available directly in the 
HTML source code.
 **Selenium:** Used if the prices and product titles are loaded dynamically via 
JavaScript.
 **Both Together:** Dynamic content is loaded with Selenium, then Beautiful 
Soup analyzes the page and pulls the data
