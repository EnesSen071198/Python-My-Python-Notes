# Tek satırlık yorumlar için '#' işareti kullanılır
# Bu yorumlar kodun ne yaptığını açıklamak için kullanılır

'''
Çok satırlı yorumlar için üç tırnak işareti kullanılır
Bu şekilde birden fazla satır yazabilirsiniz
'''

# ----- Veri Tipleri -----

# String (Metin) veri tipi
isim = "Ahmet"  # Metinsel ifadeler çift tırnak içinde yazılır
soyisim = 'Yılmaz'  # Tek tırnak da kullanılabilir
print("İsim:", isim)  # İsim: Ahmet

# Integer (Tam Sayı) veri tipi
yas = 25  # Tam sayılar direkt yazılır
dogum_yili = 1998
print("Yaş:", yas)  # Yaş: 25

# Float (Ondalıklı Sayı) veri tipi
boy = 1.78  # Ondalık sayılarda nokta kullanılır
kilo = 70.5
print("Boy:", boy)  # Boy: 1.78

# Boolean (Mantıksal) veri tipi
evli_mi = False  # True veya False değerlerini alır
ogrenci_mi = True
print("Öğrenci mi?:", ogrenci_mi)  # Öğrenci mi?: True

# Type() fonksiyonu ile veri tipini öğrenme
print(type(isim))      # <class 'str'>
print(type(yas))       # <class 'int'>
print(type(boy))       # <class 'float'>
print(type(evli_mi))   # <class 'bool'>

# ----- Tip Dönüşümleri -----

# String'den Integer'a dönüştürme
sayi_metin = "123"
sayi = int(sayi_metin)
print("Dönüştürülen sayı:", sayi + 5)  # 128

# Integer'dan String'e dönüştürme
numara = 42
numara_metin = str(numara)
print("Metin olarak: " + numara_metin)  # Metin olarak: 42

# ----- Matematiksel Operatörler -----

# Toplama işlemi (+)
sayi1 = 10
sayi2 = 5
toplam = sayi1 + sayi2
print(f"Toplam: {toplam}")  # Toplam: 15

# Çıkarma işlemi (-)
fark = sayi1 - sayi2
print(f"Fark: {fark}")  # Fark: 5

# Çarpma işlemi (*)
carpim = sayi1 * sayi2
print(f"Çarpım: {carpim}")  # Çarpım: 50

# Bölme işlemi (/)
bolum = sayi1 / sayi2
print(f"Bölüm: {bolum}")  # Bölüm: 2.0 (sonuç her zaman float olur)

# Tam sayı bölmesi (//)
tam_bolum = sayi1 // sayi2
print(f"Tam bölüm: {tam_bolum}")  # Tam bölüm: 2

# Mod alma (%)
kalan = sayi1 % sayi2
print(f"Kalan: {kalan}")  # Kalan: 0

# Üs alma (**)
us = sayi1 ** 2
print(f"10'un karesi: {us}")  # 10'un karesi: 100

# ----- Karşılaştırma Operatörleri -----

x = 10
y = 5

# Eşitlik kontrolü (==)
print(f"{x} == {y}: {x == y}")  # 10 == 5: False

# Eşit değil kontrolü (!=)
print(f"{x} != {y}: {x != y}")  # 10 != 5: True

# Büyüktür kontrolü (>)
print(f"{x} > {y}: {x > y}")    # 10 > 5: True

# Küçüktür kontrolü (<)
print(f"{x} < {y}: {x < y}")    # 10 < 5: False

# Büyük eşittir kontrolü (>=)
print(f"{x} >= {y}: {x >= y}")  # 10 >= 5: True

# Küçük eşittir kontrolü (<=)
print(f"{x} <= {y}: {x <= y}")  # 10 <= 5: False

# ----- Mantıksal Operatörler -----

a = True
b = False

# VE operatörü (and)
print(f"True and False: {a and b}")  # True and False: False

# VEYA operatörü (or)
print(f"True or False: {a or b}")    # True or False: True

# DEĞİL operatörü (not)
print(f"not True: {not a}")          # not True: False

# ----- Koşullu İfadeler (if-elif-else) -----

# Basit if kullanımı
yas = 18
if yas >= 18:
    print("Reşitsiniz")  # Reşitsiniz

# if-else kullanımı
sicaklik = 25
if sicaklik > 30:
    print("Hava sıcak")
else:
    print("Hava sıcak değil")  # Hava sıcak değil

# if-elif-else kullanımı
not_degeri = 85
if not_degeri >= 90:
    print("AA")
elif not_degeri >= 80:
    print("BA")  # BA
elif not_degeri >= 70:
    print("BB")
else:
    print("CC")

# İç içe if kullanımı
kullanici_adi = "admin"
sifre = "1234"

if kullanici_adi == "admin":
    if sifre == "1234":
        print("Giriş başarılı!")  # Giriş başarılı!
    else:
        print("Şifre yanlış!")
else:
    print("Kullanıcı adı yanlış!")

# ----- Döngüler -----

# For döngüsü - Liste üzerinde
print("\nListe üzerinde for döngüsü:")
meyveler = ["elma", "armut", "muz"]
for meyve in meyveler:
    print(f"Meyve: {meyve}")
# Çıktı:
# Meyve: elma
# Meyve: armut
# Meyve: muz

# For döngüsü - Range kullanımı
print("\nRange ile for döngüsü:")
for i in range(3):  # 0'dan 2'ye kadar
    print(f"Sayı: {i}")
# Çıktı:
# Sayı: 0
# Sayı: 1
# Sayı: 2

# While döngüsü
print("\nWhile döngüsü:")
sayac = 0
while sayac < 3:
    print(f"Sayaç: {sayac}")
    sayac += 1  # sayac = sayac + 1 ile aynı
# Çıktı:
# Sayaç: 0
# Sayaç: 1
# Sayaç: 2

# Break kullanımı (döngüyü sonlandırır)
print("\nBreak kullanımı:")
for i in range(5):
    if i == 3:
        break
    print(f"Sayı: {i}")
# Çıktı:
# Sayı: 0
# Sayı: 1
# Sayı: 2

# Continue kullanımı (döngünün o adımını atlar)
print("\nContinue kullanımı:")
for i in range(4):
    if i == 2:
        continue
    print(f"Sayı: {i}")
# Çıktı:
# Sayı: 0
# Sayı: 1
# Sayı: 3

# ----- Listeler (Lists) -----

# Liste tanımlama
meyveler = ["elma", "armut", "muz", "kiraz"]
sayilar = [1, 2, 3, 4, 5]
karisik = [1, "iki", 3.0, True]  # Farklı veri tipleri içerebilir

# Listeye erişim
print(f"İlk meyve: {meyveler[0]}")        # İlk meyve: elma
print(f"Son meyve: {meyveler[-1]}")       # Son meyve: kiraz
print(f"İlk 2 meyve: {meyveler[0:2]}")    # İlk 2 meyve: ['elma', 'armut']

# Liste metodları
meyveler.append("üzüm")          # Sona eleman ekleme
print(f"Append sonrası: {meyveler}")  # [..., 'kiraz', 'üzüm']

meyveler.insert(1, "portakal")   # İstenen konuma ekleme
print(f"Insert sonrası: {meyveler}")  # ['elma', 'portakal', 'armut', ...]

meyveler.remove("armut")         # Elemanı silme
print(f"Remove sonrası: {meyveler}")  

meyveler.pop()                   # Son elemanı çıkarma
print(f"Pop sonrası: {meyveler}")

# Liste uzunluğu
print(f"Liste uzunluğu: {len(meyveler)}")

# ----- Demetler (Tuples) -----
# Demetler listelere benzer ama değiştirilemez (immutable)

# Demet tanımlama
koordinat = (3, 5)
renkler = ("kırmızı", "mavi", "yeşil")

# Demete erişim
print(f"X koordinatı: {koordinat[0]}")  # X koordinatı: 3
print(f"İlk renk: {renkler[0]}")       # İlk renk: kırmızı

# Demet metodları
print(f"Mavi renk sayısı: {renkler.count('mavi')}")  # Mavi renk sayısı: 1
print(f"Yeşil rengin indeksi: {renkler.index('yeşil')}")  # Yeşil rengin indeksi: 2

# ----- Sözlükler (Dictionaries) -----
# Anahtar-değer çiftleri şeklinde veri saklama

# Sözlük tanımlama
ogrenci = {
    "ad": "Ahmet",
    "soyad": "Yılmaz",
    "yas": 20,
    "dersler": ["Matematik", "Fizik"]
}

# Sözlüğe erişim
print(f"Öğrenci adı: {ogrenci['ad']}")          # Öğrenci adı: Ahmet
print(f"Dersler: {ogrenci['dersler']}")         # Dersler: ['Matematik', 'Fizik']

# Sözlük metodları
print(f"Tüm anahtarlar: {ogrenci.keys()}")      # Tüm anahtarlar: ['ad', 'soyad', 'yas', 'dersler']
print(f"Tüm değerler: {ogrenci.values()}")      # Tüm değerler: ['Ahmet', 'Yılmaz', 20, ['Matematik', 'Fizik']]

# Yeni değer ekleme/güncelleme
ogrenci["bolum"] = "Bilgisayar Mühendisliği"
print(f"Ekleme sonrası: {ogrenci}")

# Get metodu ile güvenli erişim
print(f"Not ortalaması: {ogrenci.get('ortalama', 'Bilgi yok')}")  # Bilgi yok

# Sözlükten değer silme
del ogrenci["yas"]
print(f"Silme sonrası: {ogrenci}")

# ----- Fonksiyonlar -----

# Basit fonksiyon tanımlama
def selamla():
    print("Merhaba!")

# Fonksiyonu çağırma
selamla()  # Merhaba!

# Parametreli fonksiyon
def kisi_selamla(isim):
    print(f"Merhaba {isim}!")

kisi_selamla("Ahmet")  # Merhaba Ahmet!

# Varsayılan parametreli fonksiyon
def selamla_dil(isim, dil="TR"):
    if dil == "TR":
        print(f"Merhaba {isim}!")
    elif dil == "EN":
        print(f"Hello {isim}!")

selamla_dil("Ahmet")        # Merhaba Ahmet!
selamla_dil("John", "EN")   # Hello John!

# Değer döndüren fonksiyon
def topla(a, b):
    return a + b

sonuc = topla(5, 3)
print(f"Toplam: {sonuc}")  # Toplam: 8

# Birden fazla değer döndüren fonksiyon
def geometrik_hesapla(yaricap):
    """
    Dairenin çevre ve alanını hesaplar
    Args:
        yaricap: Dairenin yarıçapı
    Returns:
        cevre, alan: Dairenin çevresi ve alanı
    """
    pi = 3.14
    cevre = 2 * pi * yaricap
    alan = pi * yaricap ** 2
    return cevre, alan

cevre, alan = geometrik_hesapla(5)
print(f"Çevre: {cevre}, Alan: {alan}")

# ----- Hata Yakalama (Try-Except) -----

# Basit try-except kullanımı
try:
    sayi = int(input("Bir sayı girin: "))
    print(f"Girdiğiniz sayı: {sayi}")
except ValueError:
    print("Lütfen geçerli bir sayı girin!")

# Birden fazla hata yakalama
try:
    sayi1 = int(input("Birinci sayı: "))
    sayi2 = int(input("İkinci sayı: "))
    bolum = sayi1 / sayi2
    print(f"Bölüm: {bolum}")
except ValueError:
    print("Lütfen geçerli bir sayı girin!")
except ZeroDivisionError:
    print("Bir sayı sıfıra bölünemez!")
except Exception as e:
    print(f"Bir hata oluştu: {e}")
finally:
    print("İşlem tamamlandı!")

# Kendi hata sınıfımızı oluşturma
class YasHatasi(Exception):
    pass

def yas_kontrol(yas):
    if yas < 0:
        raise YasHatasi("Yaş negatif olamaz!")
    elif yas > 120:
        raise YasHatasi("Geçersiz yaş değeri!")
    else:
        print(f"Yaşınız: {yas}")

# Özel hata sınıfını kullanma
try:
    yas_kontrol(150)
except YasHatasi as e:
    print(f"Hata: {e}")

# Assert kullanımı (Hata ayıklama amaçlı)
def kare_al(sayi):
    assert sayi >= 0, "Negatif sayının karesi alınamaz!"
    return sayi ** 2

try:
    print(kare_al(-5))
except AssertionError as e:
    print(f"Hata: {e}")

# ----- Dosya İşlemleri -----

# Dosya yazma (write - 'w' modu)
with open("notlar.txt", "w", encoding="utf-8") as dosya:
    dosya.write("Python Öğreniyorum\n")
    dosya.write("Dosya işlemleri konusundayım\n")

# Dosyaya ekleme yapma (append - 'a' modu)
with open("notlar.txt", "a", encoding="utf-8") as dosya:
    dosya.write("Bu satır sonradan eklendi\n")

# Dosya okuma (read - 'r' modu)
with open("notlar.txt", "r", encoding="utf-8") as dosya:
    icerik = dosya.read()
    print("Dosya içeriği:")
    print(icerik)

# Satır satır okuma
with open("notlar.txt", "r", encoding="utf-8") as dosya:
    for satir in dosya:
        print(f"Satır: {satir.strip()}")

# ----- Modüller -----

# Math modülünü import etme
import math

# Matematik işlemleri
print(f"Pi sayısı: {math.pi}")
print(f"5'in karekökü: {math.sqrt(25)}")
print(f"5'in faktöriyeli: {math.factorial(5)}")

# Random modülü
import random

# Rastgele sayı üretme
print(f"1-10 arası rastgele sayı: {random.randint(1, 10)}")
liste = ["elma", "armut", "muz"]
print(f"Listeden rastgele seçim: {random.choice(liste)}")

# Datetime modülü
from datetime import datetime, timedelta

# Tarih ve saat işlemleri
simdi = datetime.now()
print(f"Şu an: {simdi}")
print(f"Yıl: {simdi.year}, Ay: {simdi.month}, Gün: {simdi.day}")

# 5 gün sonrası
bes_gun_sonra = simdi + timedelta(days=5)
print(f"5 gün sonra: {bes_gun_sonra}")

# ----- Nesne Yönelimli Programlama (OOP) -----

# Sınıf tanımlama
class Araba:
    # Sınıf değişkeni
    uretilen_arac_sayisi = 0
    
    # Constructor (Yapıcı) metod
    def __init__(self, marka, model, yil):
        self.marka = marka  # Instance değişkeni
        self.model = model
        self.yil = yil
        self.hiz = 0
        Araba.uretilen_arac_sayisi += 1
    
    # Instance metodu
    def hizlan(self, artis):
        self.hiz += artis
        print(f"Hız: {self.hiz} km/saat")
    
    def yavasla(self, azalis):
        self.hiz = max(0, self.hiz - azalis)
        print(f"Hız: {self.hiz} km/saat")
    
    # String temsili
    def __str__(self):
        return f"{self.yil} model {self.marka} {self.model}"
    
    # Class metodu
    @classmethod
    def arac_sayisi(cls):
        return f"Toplam {cls.uretilen_arac_sayisi} araç üretildi"

# Kalıtım (Inheritance)
class ElektrikliAraba(Araba):
    def __init__(self, marka, model, yil, batarya_kapasitesi):
        super().__init__(marka, model, yil)
        self.batarya_kapasitesi = batarya_kapasitesi
        self.sarj_durumu = 100
    
    def sarj_et(self):
        self.sarj_durumu = 100
        print("Batarya tam şarj edildi")

# Sınıfları kullanma
araba1 = Araba("Toyota", "Corolla", 2020)
araba2 = ElektrikliAraba("Tesla", "Model 3", 2022, 75)

print(araba1)  # 2020 model Toyota Corolla
araba1.hizlan(50)  # Hız: 50 km/saat
araba1.yavasla(20)  # Hız: 30 km/saat

print(araba2)  # 2022 model Tesla Model 3
araba2.sarj_et()  # Batarya tam şarj edildi

print(Araba.arac_sayisi())  # Toplam 2 araç üretildi

# ----- Dekoratörler -----

# Fonksiyon dekoratörü
def zaman_olc(fonksiyon):
    def wrapper(*args, **kwargs):
        baslangic = datetime.now()
        sonuc = fonksiyon(*args, **kwargs)
        bitis = datetime.now()
        print(f"{fonksiyon.__name__} fonksiyonu {bitis - baslangic} sürede çalıştı")
        return sonuc
    return wrapper

# Dekoratör kullanımı
@zaman_olc
def faktoriyel(n):
    return math.factorial(n)

print(f"Faktöriyel sonucu: {faktoriyel(10)}")

# ----- List Comprehension -----

# Normal liste oluşturma
kareler = []
for i in range(5):
    kareler.append(i ** 2)
print(f"Kareler: {kareler}")

# List comprehension ile
kareler2 = [i ** 2 for i in range(5)]
print(f"Kareler (comprehension): {kareler2}")

# Koşullu list comprehension
cift_sayilar = [i for i in range(10) if i % 2 == 0]
print(f"Çift sayılar: {cift_sayilar}")
