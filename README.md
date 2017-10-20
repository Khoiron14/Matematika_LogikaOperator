# Operator Logika PHP
Operator logika digunakan untuk membandingkan tipe data boolean, yaitu true(benar), dan false(salah). Operator logika sering dipakai untuk struktur
kontrol, kondisi if ataupun looping.

### Contoh Operator Logika
![Operatorlogika.jpg](http://blog.mitschool.co.id/wp-content/uploads/2017/04/Logical-Operator.jpg)

#### Operator AND (&&)
Operator &&, operator ini akan menghasilkan nilai true jika kedua kondisi benar (bernilai true).

Cara penggunaan :
```PHP
$a = 2;
$b = 2;
if ($a && $b == 2) {
    echo "variable $a dan $b berisi 2";
}
```
Kode diatas akan memunculkan pesan "angka sama", karena variable $a maupun $b berisi 2;
- Jika salah satu variable nilainya bukan 2 maka akan bernilai false, dan if tidak dijalankan.

#### Operator OR (||)
Operator ||, operator ini akan menghasilkan nilai true apabila salah satu kondisi benar (bernilai true).

Cara penggunakan :
```PHP
$a = 2;
$b = 5;
if ($a || $b == 2) {
    echo "kondisi bernilai TRUE";
}
```
Kode diatas akan memunculkan pesan "kondisi bernilai TRUE", karena salah satu variable memiliki nilai 2.
- IF akan bernilai true apabila dua atau salah satu kondisi bernilai TRUE.

#### Operator NOT (!)
Operator !, operator ini akan menghasilkan nilai TRUE apabila suatu kondisi bernilai salah (FALSE). Operator ini adalah operator kebalikan.

```PHP
$a = 7;
if ($a != 2) {
    echo "variable $a tidak berisi 2";
}
```
Kode diatas akan memunculkan pesan "variable $a tidak berisi 2", karena isi variable $a bukan 2.

#### Operator NAND (!(&&))
Operator !(&&), adalah gabungan dari AND dan NOT, operator ini merupakan kebalikan dari operator AND.
```PHP
$a = 2;
$b = 3;
if (!($a && $b)) {
    echo "kondisi bernilai TRUE";
}
```

#### Operator XOR (^)
Operator ^, operator ini akan menghasilkan nilai TRUE apabila salah satu dari kondisi bernilai TRUE, tapi bukan keduanya.
```PHP
$a = 2;
$b = 3;
if ($a ^ $b == 2) {
    echo "salah satu variable bernilai 2";
}
```
Kode diatas akan memunculkan pesan "salah satu variable bernilai 2", karena salah satu variable bernilai 2.
- Jika kedua variable diatas bernilai 2, maka kondisi tersebut bernilai FALSE.

#### Operator XNOR !(^)
Operator , Operator ini akan menghasilkan nilai TRUE jika kedua kondisi bernilai sama, TRUE atau FALSE.
```PHP
$a = 2;
$b = 2;
if (!($a ^ $b == 2)) {
    echo "salah satu variable bernilai 2";
}
```
- IF akan bernilai false apabila kedua variable diatas bernilai berbeda.
