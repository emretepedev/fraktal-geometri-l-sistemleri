# Onbilgi
Bu repository Fraktal Geometri dersi icin hazirlanmis odev kodlarini icerir. https://emretepedev.github.io/fraktal-geometri-l-sistemleri/ adresinden goruntulenebilir. Herhangi bir PR kabul edilmeyecektir. Dersin egitmeni, bu application'in derslerde kendi tarafindan kullanilacagini beyan etmesi sebebiyle sadece GitHub Pages uzerinde yayinlanmasi amaciyla bulunmaktadir.

# Nasil Calisir

L sistemleri, bitkilerin buyume/yayilmalarini modellemek amaciyla lindmayer tarafindan gelistirilen gramer tabanli sistemdir.

L sistemleri 3 ana bilesene ihtiyac duyar:
1. Alfabe: Cumle icinde gecerli olacak karakterler kumesi. Ornegin, eger alfabe “ABC” ise herhangi gecerli cumle A, B, C kelimelerini icerecektir.
2. Aksiyom: Sistemin ilk durumunu aciklayan cumle. Ornegin, alfabe “ABC,” ise bazi ornek aksiyomlar sunlar olabilir: “AAA” veya “B” veya “ACBAB.”
3. Olusum Kurallari: Aksiyom cumlesi ile baslayip, ozyinelemeli olarak yeni cumleler olusturulmak ve uygulanmak uzere belirlenecek kurallar butunu. Ornegin, kuralimiz “A → AB” ise sistem, metin icerisinde ”A” bulmali ve bunu “AB” ile degistirmeli.

* Opsiyonel olarak olusturulacak fraktala bagli olarak parametre degiskenine de ihtiyac duyariz. Ornegin, eger sistemimizi olustururken alfabemiz icinde +, - ifadeleri yer aliyorsa, α acisini parametre olarak bildirmeliyiz.

Ornek:

Alfabe: A B

Aksiyom: A

Olusum Kurallari: ( A → ABA ) ( B → BBB )

A: Bir cizim yaparak ilerlemek

B: Herhangi bir cizim yapmadan ilerlemek

Olusum Asamasi 0: A

Olusum Asamasi 1: ABA

Olusum Asamasi 2: ABABBBABA

Olusum Asamasi 3: ABABBBABABBBBBBBBBABABBBA

Alfabe icinde yer alabilecek bazi ozel sozdizimleri de mevcuttur.

+: α acisi kadar saga don

-: α acisi kadar sola don

[: Mevcut pozisyonu kaydet

]: Kaydedilen son pozisyona don

* Programlama tarafinda merak edenler icin Python ortaminda https://github.com/hhassen/L-system repository kullanabilirler.

# Gelistirme ortaminin hazirlanmasi

### Install

```
npm install
npm install webpack-dev-server webpack -g
```

### Serve

To serve at http://localhost:8080/:

```
npm start
```

or

```
webpack-dev-server --inline  --content-base public/
```

### Build

```
npm run build
```

or

```
webpack --config webpack.config.js
```
