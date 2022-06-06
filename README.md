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