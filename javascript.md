# 🟨 JavaScript Cheatsheet (ES6+)

## Değişkenler

```javascript
const sabit = 10;           // Sabit değer
let degisen = 20;           // Değişken değer
// var eskiYontem = 30;     // Kullanmayın!
```

## Fonksiyonlar

```javascript
// Arrow function
const merhaba = (isim) => `Merhaba ${isim}!`;

// Default parameter
const selamla = (isim = "Dünya") => `Selam ${isim}!`;

// Rest parameter
const topla = (...sayilar) => sayilar.reduce((a, b) => a + b, 0);
```

## Destructuring

```javascript
// Array
const [bir, iki] = [1, 2, 3];

// Object
const { ad, yas } = { ad: "Ali", yas: 25, sehir: "İstanbul" };

// Nested
const { adres: { sehir } } = { adres: { sehir: "Ankara" } };
```

## Array Methods

```javascript
const sayilar = [1, 2, 3, 4, 5];

sayilar.map(x => x * 2);        // [2, 4, 6, 8, 10]
sayilar.filter(x => x > 3);     // [4, 5]
sayilar.reduce((a, b) => a + b); // 15
sayilar.find(x => x > 3);       // 4
sayilar.some(x => x > 3);       // true
sayilar.every(x => x > 0);      // true
```

## Async/Await

```javascript
const veriGetir = async () => {
  try {
    const cevap = await fetch("https://api.example.com/data");
    const veri = await cevap.json();
    return veri;
  } catch (hata) {
    console.error("Hata:", hata);
  }
};
```

## Spread & Rest

```javascript
// Spread
const dizi1 = [1, 2, 3];
const dizi2 = [...dizi1, 4, 5]; // [1, 2, 3, 4, 5]

const obje1 = { a: 1, b: 2 };
const obje2 = { ...obje1, c: 3 }; // { a: 1, b: 2, c: 3 }
```
