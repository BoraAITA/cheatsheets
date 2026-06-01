# 🐍 Python Cheatsheet

## Temel Syntax

```python
# Değişkenler
isim = "Ali"                 # String
yas = 25                     # Integer
boy = 1.75                   # Float
aktif = True                 # Boolean
liste = [1, 2, 3]            # List
sozluk = {"anahtar": "değer"}  # Dict
kume = {1, 2, 3}             # Set
```

## Kontrol Yapıları

```python
# If/Else
if kosul:
    pass
elif baska_kosul:
    pass
else:
    pass

# For döngüsü
for i in range(10):
    print(i)

# While
while kosul:
    break
```

## Fonksiyonlar

```python
# Normal fonksiyon
def merhaba(isim):
    return f"Merhaba {isim}!"

# Lambda
topla = lambda x, y: x + y

# Default parameter
def selamla(isim="Dünya"):
    return f"Selam {isim}!"

# *args ve **kwargs
def fonksiyon(*args, **kwargs):
    pass
```

## List Comprehension

```python
# Temel
kareler = [x**2 for x in range(10)]

# Koşullu
ciftler = [x for x in range(20) if x % 2 == 0]

# İç içe
matrix = [[j for j in range(3)] for i in range(3)]
```

## Dosya İşlemleri

```python
# Okuma
with open("dosya.txt", "r") as f:
    icerik = f.read()

# Yazma
with open("dosya.txt", "w") as f:
    f.write("Merhaba Dunya!")

# Satır satır okuma
with open("dosya.txt") as f:
    for satir in f:
        print(satir.strip())
```

## Hata Yönetimi

```python
try:
    sonuc = 10 / 0
except ZeroDivisionError as e:
    print(f"Hata: {e}")
except Exception as e:
    print(f"Beklenmeyen hata: {e}")
finally:
    print("Her durumda çalışır")
```

## Class

```python
class Kiisi:
    def __init__(self, isim, yas):
        self.isim = isim
        self.yas = yas
    
    def tanit(self):
        return f"Ben {self.isim}, {self.yas} yaşındayım."
```

## İpuçları

```python
# f-string (Python 3.6+)
isim = "Ali"
yas = 25
print(f"Merhaba {isim}, {yas} yaşındasın.")

# Walrus operator (Python 3.8+)
if (n := len("merhaba")) > 5:
    print(f"Uzunluk: {n}")

# Unpacking
a, b, *geri = [1, 2, 3, 4, 5]
```
